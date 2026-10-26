#include <iostream>
#include <ctime> //we included this library to use ctime functions
#include <stdlib.h> //we include this library to use system("pause")
using namespace std;

int stars(int i) //first subfunction to print '*' using for loop
{
    for(int n=0; n<i; n++)
    {
        cout<<"*";
    }
    cout<<endl;
}

int space(int i) //second subfunction to print ' ' using for loop
{
    for(int n=0; n<i; n++)
    {
        cout<<endl;
    }
}

int score(int ending) //third subfunction to print objectives achieved and scores according to the ending user obtains.
{
    space(2); //an example of calling second subfunction in third subfunction
    stars(20);
    space(1);
    cout<<"THE END"<<endl;
    space(1);
    cout<<"Score will now be given based on the ending you have gained, how safe are your choices/actions and good luck. There are a total of 12th endings available."<<endl;\
    cout<<"THE ENDING YOU HAVE ACHIEVED IS THE ENDING NUMBER "<<ending<<endl;
    switch (ending) //use of switch
    {
    case 1:
        cout<<"0/2 OJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 8.33%"<<endl;
        break;
    case 2:
        cout<<"1/2 OBJECTIVE ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 75.0%"<<endl;
        break;
    case 3:
        cout<<"0/2 OJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 41.67%"<<endl;
        break;
    case 4:
        cout<<"2/2 OBJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 91.60%"<<endl;
        break;
    case 5:
        cout<<"1/2 OBJECTIVE ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 66.67%"<<endl;
        break;
    case 6:
        cout<<"0/2 OJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 16.67%"<<endl;
        break;
    case 7:
        cout<<"0/2 OJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 50.0%"<<endl;
        break;
    case 8:
        cout<<"2/2 OBJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 100.0%"<<endl;
        break;
    case 9:
        cout<<"1/2 OBJECTIVE ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 58.3%"<<endl;
        break;
    case 10:
        cout<<"0/2 OJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 25.0%"<<endl;
        break;
    case 11:
        cout<<"2/2 OBJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 83.33%"<<endl;
        break;
    case 12:
        cout<<"0/2 OJECTIVES ACHIEVED."<<endl;
        cout<<"TOTAL SCORE: 33.33%"<<endl;
        break;
    }
}

//base class
class plot //use of classes; this is a base class
{
public:
    void options()
    {
        int ending;
        space(2); //an example of calling second subfunction in a base class
        cout<<"You are watching the television in your living room when someone knocks on the door. Your parents are out."<<endl;
        space(2);
        cout<<"/Hint: Your parents have not informed of anyone visiting./"<<endl;

        CHOICE_DOOR: //using this so we could use jump statements like 'goto'
            space(4);
            char door;
            cout<<"OPEN THE DOOR? 'Y' FOR YES, 'N' FOR NO: >> "; //user enters the wanted input according to their wanted actions; (if they want to say yes, enter 'Y')
            cin>>door;
            if (door=='Y') //one of the many if-else used in the program; a long and many nested if else followed. used for outputs for actions depending on users' input (action to take)
            {
                space(4);
                cout<<"Your parents aren't home, but perhaps your neighbor is at the door."<<endl;
                space(2);
                cout<<"Just in case, you should at least check out if it could be your neighbor..."<<endl;

                LUCK1:
                    int luck1; //for variables named 'luck', user is to input 1 or 2; one of them set as bad luck and the other set as good luck
                    space(4);
                    cout<<"LUCK: 1 OR 2? >> ";
                    cin>>luck1;
                    if (luck1==1) //Bad Luck
                    {
                        space(4);
                        cout<<"Jokes on you; the stranger who's choking you currently is anything but your neighbor..."<<endl;
                        int ending=1;
                        score(ending);
                    }
                    else if (luck1==2) //Good Luck
                    {
                        space(4);
                        cout<<"You let out the breath that you were unconsciously holding when it is, in fact, your neighbor at the door."<<endl;
                        int ending=2;
                        score(ending);
                    }
                    else //this part is not mandatory, but to ensure program runs smoothly and the correct output will be displayed, any inputs that differ from the instruction will be asked for again
                    {
                        space(4);
                        cout<<"TRY AGAIN"<<endl;
                        goto LUCK1; //use of 'goto' because users enter the wrong input (most common mistake would be inputting 'a' when asked of 'A')
                    }
            }
            else if (door=='N')
            {
                space(4);
                cout<<"Indeed, you ought to stay cautious. Your parents didn't tell you anything about anyone visiting..."<<endl;
                space(2);
                cout<<"Although, it is better if you know who is at the door. So you peek through the window."<<endl;
                space(2);
                cout<<"You instantly back away after meeting eyes with a stranger, an unsettling grin on his lips."<<endl;

                CHOICE_HIDE:
                    char hide;
                    space(4);
                    cout<<"HIDE! BUT WHERE...?"<<endl<<" >>A: Kitchen"<<endl<<" >>B: Bedroom"<<endl<<" >>C: Toilet"<<endl<<" >>> ";
                    cin>>hide;
                    if (hide=='A')
                    {
                        space(4);
                        cout<<"Kitchen does seem like a good choice. You would be able to get something to protect yourself with and would be able to escape through the back door."<<endl;

                        LUCK2:
                            int luck2;
                            space(4);
                            cout<<"LUCK: 1 OR 2? >> "<<endl;
                            cin>>luck2;
                            if (luck2==1) //Bad Luck
                            {
                                space(4);
                                cout<<"Huh... You forgot the stranger has eyes too... There he is, standing inside your kitchen, a creepy grin on his face."<<endl;
                                int ending=3;
                                score(ending);
                            }
                            else if (luck2==2) //Good Ending
                            {
                                space(4);
                                cout<<"You quickly grab a knife for defense. In this day and age, everyone always carry their phones around. You quickly dial 911."<<endl;
                                space(2);
                                cout<<"Just when you thought you are safe, you see the stranger staring through the back door."<<endl;

                                CHOICE_BACKDOOR:
                                    char backdoor;
                                    space(4);
                                    cout<<"DO YOU..."<<endl<<" >>A: Hide in the bedroom. Although it may be futile, you would lock the door and windows..."<<endl<<" >>B: Stay standing and keep an eye on the stranger until help arrives to arrest the stranger."<<endl<<" >>> ";
                                    cin>>backdoor;
                                    if (backdoor=='A')
                                    {
                                        space(4);
                                        cout<<"Even as you hear footsteps outside the room, you pretend to not hear them, focusing on calming yourself."<<endl;
                                        space(2);
                                        cout<<"The door knob rattles  a few times, yet the stranger gives up quite fast; his footsteps going around the house except for the bedroom."<<endl;
                                        space(2);
                                        cout<<"Eventually, help arrives, but the stranger is nowhere in sight..."<<endl;
                                        int ending=4;
                                        score(ending);
                                    }
                                    else if (backdoor=='B')
                                    {
                                        space(4);
                                        cout<<"The thought of this stranger fleeing when help arrives irks you. So you did what anyone would be doing in your situation:"<<endl;
                                        space(2);
                                        cout<<"Keeping an eye on the stranger and basically have a staring contest with him."<<endl;

                                        LUCK3:
                                            int luck3;
                                            space(4);
                                            cout<<"LUCK: 1 OR 2? >> ";
                                            cin>>luck3;
                                            if (luck3==1) //Good Luck
                                            {
                                                space(4);
                                                cout<<"You are lucky the stranger is kind of a noob; help arrives and manages to arrest the stranger. Although, the entertained and a little crazed grin he gives you as he is taken away is quite disturbing..."<<endl;
                                                int ending=5;
                                                score(ending);
                                            }
                                            else if (luck3==2) //Bad luck
                                            {
                                                space(4);
                                                cout<<"Despite probably knowing that you have called for help, the stranger seems to not care, eyes train on you."<<endl;
                                                space(2);
                                                cout<<"The stranger looks so at peace, you start to wonder if... he has a backup plan..."<<endl;
                                                space(2);
                                                cout<<"While you start to ponder and think, you are unaware of the back door knob's turning, unlocking the door..."<<endl;
                                                int ending=6;
                                                score(ending);
                                            }
                                            else
                                            {
                                                space(4);
                                                cout<<"TRY AGAIN"<<endl;
                                                goto LUCK3;
                                            }
                                    }
                                    else
                                    {
                                        space(4);
                                        cout<<"TRY AGAIN"<<endl;
                                        goto CHOICE_BACKDOOR;
                                    }
                            }
                            else
                            {
                                space(4);
                                cout<<"TRY AGAIN"<<endl;
                                goto LUCK2;
                            }
                    }
                    else if (hide=='B')
                    {
                        space(4);
                        cout<<"You panicked. The stranger may try to enter through the back door. The bedroom would probably has the most hiding spots in the house..."<<endl;

                        CHOICE_SPOT:
                            char spot;
                            space(4);
                            cout<<"WHERE WOULD YOU HIDE?"<<endl<<" >>A: Closet"<<endl<<" >>B: Under the bed"<<endl<<" >>C: Not hide, instead..."<<endl<<" >>> ";
                            cin>>spot;
                            if (spot=='A' || spot=='B') //use of '||' which means OR
                            {
                                LUCK4:
                                    int luck4;
                                    space(4);
                                    cout<<"LUCK: 1 OR 2? >> ";
                                    cin>>luck4;
                                    if (luck4==1) //Bad Luck
                                    {
                                        space(4);
                                        cout<<"Unfortunately, it is already too late when help arrives; the stranger had plenty of time to search for you."<<endl;
                                        space(2);
                                        cout<<"...and search he did..."<<endl;
                                        int ending=7;
                                        score(ending);
                                    }
                                    else if (luck4==2) //Good Luck
                                    {
                                        space(4);
                                        cout<<"You hide as well as you could. Before the stranger could find you, help arrives."<<endl;
                                        int ending=8;
                                        score(ending);
                                    }
                                    else
                                    {
                                        space(4);
                                        cout<<"TRY AGAIN"<<endl;
                                        goto LUCK4;
                                    }
                            }
                            else if (spot=='C')
                            {
                                CHOICE_SURE:
                                    char sure;
                                    space(4);
                                    cout<<"ARE YOU SURE?"<<endl<<" >>Y: Yes."<<endl<<" >>N: No."<<endl<<" >>> ";
                                    cin>>sure;
                                    if (sure=='N')
                                    {
                                        goto CHOICE_SPOT;
                                    }
                                    else if (sure=='Y')
                                    {
                                        space(4);
                                        cout<<"Although risky, you have decided to risk it and hide behind the door, armed with a bat in the room and waiting for the stranger to enter so you could swing."<<endl;

                                        LUCK5:
                                            int luck5;
                                            space(4);
                                            cout<<"LUCK: 1 OR 2? >> ";
                                            cin>>luck5;
                                            if (luck5==1) //Good Luck
                                            {
                                                cout<<space(4)<<endl;
                                                cout<<"With precise timing and sheer luck, you are able to knock and stagger the stranger as soon as he entered. You quickly run through the door, seeking help from your neighbor..."<<endl;
                                                int ending=9;
                                                score(ending);
                                            }
                                            else if (luck5==2) //Bad Luck
                                            {
                                                space(4);
                                                cout<<"You shouldn't have underestimated the stranger..."<<endl;
                                                space(2);
                                                cout<<"As soon as the door is opened, you freezes in fear, noticing how it seems that you aren't his first victim..."<<endl;
                                                int ending=10;
                                                score(ending);
                                            }
                                            else
                                            {
                                                space(4);
                                                cout<<"TRY AGAIN"<<endl;
                                                goto LUCK5;
                                            }
                                    }
                                    else
                                    {
                                        space(4);
                                        cout<<"TRY AGAIN"<<endl;
                                        goto CHOICE_SURE;
                                    }
                            }
                            else
                            {
                                space(4);
                                cout<<"TRY AGAIN"<<endl;
                                goto CHOICE_SPOT;
                            }
                    }
                    else if (hide=='C')
                    {
                        space(4);
                        cout<<"You run straight for the toilet, with nothing to arm yourself with..."<<endl;

                        LUCK6:
                            int luck6;
                            space(4);
                            cout<<"LUCK: 1 OR 2? >> ";
                            cin>>luck6;
                            if (luck6==1) //Good Luck
                            {
                                space(4);
                                cout<<"Somehow, you only hear footsteps, yet those footsteps sound far. When help arrives, a few items are gone, but at least your life isn't..."<<endl;
                                int ending=11;
                                score(ending);
                            }
                            else if (luck6==2) //Bad Luck
                            {
                                space(4);
                                cout<<"You barely get to breathe when the sound of the door unlocked and fast footsteps follow you..."<<endl;
                                int ending=12;
                                score(ending);
                            }
                            else
                            {
                                space(4);
                                cout<<"TRY AGAIN"<<endl;
                                goto LUCK6;
                            }
                    }
                    else
                    {
                        space(4);
                        cout<<"TRY AGAIN"<<endl;
                        goto CHOICE_HIDE;
                    }
            }
            else
            {
                space(4);
                cout<<"TRY AGAIN"<<endl;
                goto CHOICE_DOOR;
            }
    }
};

//derived class for options
class flow : public plot //use of classes; this is a derived class
{
public:
    void storyline()
    {
        cout<<endl;
    }
};

void house_layout() //fourth subfunction to print the house's layout of the character the user would be playing as
{
    string frontyard[3]={"     ","*DOOR*","      "}; //a lot of usage of arrays
    string second_level[2]={"* living *","* kitchen *"};
    string second_level_pt2[2]={"*  room  *","*         *"};
    string third_level[3]={"* Toi *"," Bed  ","*DOOR*"};
    string third_level_pt2[3]={"* let *"," room ","******"};
    cout<<"     "<<"******"<<"      "<<endl;
    cout<<frontyard[0]<<frontyard[1]<<frontyard[2]<<endl; //a lot of usage of calling and printing elements of arrays
    cout<<"*********************"<<endl;
    cout<<second_level[0]<<second_level[1]<<endl;
    cout<<second_level_pt2[0]<<second_level_pt2[1]<<endl;
    cout<<"*********************"<<endl;
    cout<<"*******************"<<endl;
    cout<<third_level[0]<<third_level[1]<<third_level[2]<<endl;
    cout<<third_level_pt2[0]<<third_level_pt2[1]<<third_level_pt2[2]<<endl;
    cout<<"**************"<<endl;

}

void pause() //fifth subfunction to use the system("pause") function so the game becomes more user-engaging
{
    cout<<endl;
    system("pause"); //a function from <stdlib.h> library
    cout<<endl;
}

//main function
int main()
{
    time_t start; //another feature we could use by including <ctime>
    time(&start);  //recording the starting time/ starting a timer as comments will be given based on the time user take to complete the game

    //Time the game is started
    time_t current_time;
	current_time = time(NULL);

	char* now1 = ctime(&current_time); //use of pointer
	cout << "NOW IS " << now1; //display the date, month, year, hour, minute and seconds.

    START:
    space(1); //an example of calling the second subfunction in main function
    stars(20);
    cout<<"WELCOME TO"<<endl;
    string cye[3]={"CHOOSE","*YOUR*","ENDING"};
    cout<<cye[0]<<endl<<cye[1]<<endl<<cye[2]<<endl;
    cout<<endl;
    stars(20);
    pause();
    cout<<"This is a user-dependent game, where you are to be assigned a role and have to achieve certain objectives."<<endl;
    space(1);
    cout<<"Remember, luck may play a part in achieving the objectives."<<endl;
    pause();
    space(1);
    cout<<"OBJECTIVES:"<<endl;
    cout<<"1)DO NOT get caught."<<endl;
    cout<<"2)Escape SAFELY."<<endl;
    pause();
    space(1);
    house_layout();
    pause();
    space(1);
    cout<<"One last reminder; this game is case-sensitive. (eg. 'a' is different than 'A')"<<endl;
    space(1);
    stars(20);
    //Create object of derived class
    flow output;
    //Calling members of the base class
    output.options();
    //scores();

    REPEAT:
    char repeat;
    space(2);
    cout<<"WOULD YOU LIKE TO TRY AGAIN FROM THE TOP? 'Y' FOR YES and 'N' FOR NO: ";
    cin>>repeat;
    if (repeat=='Y')
    {
        goto START;
    }
    else if (repeat=='N')
    {
        goto END;
    }
    else
    {
        space(4);
        cout<<"TRY AGAIN"<<endl;
        goto REPEAT;
    }

    END:

    time_t finish;
    time(&finish); //recording the time the game ended/ ending the timer

    //Time the game is ended
    time_t current_time2;
	current_time2 = time(NULL);

	char* now2 = ctime(&current_time2);
	space(2);
	cout << "NOW IS " << now2; //display the date, month, year, hour, minute and seconds.

	double time_taken=difftime(finish,start); //a function from library <ctime>. differentiate the time the timer ended with the time the timer started
	cout<<"YOU HAVE SPENT "<<time_taken<<" SECONDS PLAYING THE GAME!!"<<endl; //display the time taken to finish the game

	if (time_taken<=30)
    {
        space(2);
        cout<<"WOW!! YOU ARE A QUITE DECISIVE PERSON! QUICK THINKING TOO! IF YOU ARE INTERESTED IN MORE GAMES LIKE THIS ONE, ONE OF OUR TEAM MEMBERS HAVE MADE A GAME SIMILAR TO THIS ONE; EXCEPT IT OFFERS 3 ROLES AND HAS A TOTAL OF 36 ENDINGS! PLUS, THE STORY IS MORE INTRICATE AND DETAILED COMPARED TO THIS ONE!! IF INTERESTED, FEEL FREE TO ASK FOR IT!!"<<endl;
        space(1);
        cout<<"ALTHOUGH, IT IS NOT GUARANTEED THAT YOU WOULD GET IT..."<<endl;
        space(1);
        cout<<"MAKING AN EFFORT IS NICE THOUGH!"<<endl;
    }
    else if (time_taken>30 && time_taken<=60) //use of '&&' which means AND
    {
        space(2);
        cout<<"FOR A SIMPLE GAME LIKE THIS ONE, IT'S QUITE NORMAL TO TAKE THIS LONG! WELL DONE!"<<endl;
    }
    else if (time_taken>60)
    {
        space(2);
        cout<<"...YOU PROBABLY TOOK THIS LONG FOR ONE OF THESE REASONS:"<<endl;
        cout<<">> A) IT'S YOUR FIRST TIME PLAYING AND YOU TOOK YOUR TIME UNDERSTANDING THE INSTRUCTIONS."<<endl;
        cout<<">> B) YOU ARE JUST AN INDECISIVE PERSON/ YOU TOOK YOUR SWEET TIMES CHOOSING YOUR ACTIONS..."<<endl;
        cout<<">> C) YOU ARE CURRENTLY PRESENTING HOW EVERYTHING WORKS IN DETAILS TO SOMEONE..."<<endl;
        cout<<">> D) YOU HAD A HARD TIME COMPREHENDING CERTAIN ELEMENTS (EG. ENGLISH, ENVISIONING WHAT'S HAPPENING, ETC.)"<<endl;
        cout<<">> E) YOU REPEATED THE GAME MANY TIMES."<<endl;
        space(1);
        cout<<"EITHER WAY, YOU STILL MANAGED TO COMPLETE THE GAME UNTIL THE END!! WELL DONE!"<<endl;
    }

    space(2);
    stars(20);
    cout<<"THANK YOU FOR PLAYING!"<<endl;
    space(1);
    stars(20);
    return 0;
}
