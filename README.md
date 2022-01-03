# Personal-Assistant-application
C++ voice assistant(AKA sasta jarvis). 


Included these 4 lines of code for the text to speech feature:

string phrase = "whatever message you want to listen to";
string command = "espeak \"" + phrase + "\"";
const char *charCommand = command.c_str();
system(charCommand);

To open any file format in the system, the command is:
ShellExecute(NULL,"open","file path",NULL, NULL, SW_NORMAL);

To open a browser:
system("start url of browser");
Example:
system("start https://www.youtube.com");

To open .exe files such as ms word,paint,excel notepad etc:
CreateProcess(TEXT("file path"), NULL, NULL, NULL, FALSE, NULL, NULL, NULL, &startInfo, &processInfo);


