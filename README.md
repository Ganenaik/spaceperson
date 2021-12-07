
#include<iostream>
#include<fstream>
#include<string>
 
using namespace std;

bool IsloggedIn()
{
    String username , passoword, un, pw;
    cout<<"Enter a username"<<endl;
    cin>>username;
    cout<<"Enter a password"<<endl;
    cin>>password;
    
  ifstream read ("c:\\" + username + ".txt");
    getline(read,un);
    getline(read,pw);
    
    if(un==username && pw == password )
    {
        return true;
        
    }
        
        else{
            return false ;
        }
    }
    int main()
    {
        int choice ;
        cout<<"1.Register\n 2.Login\nyourchoice"<<endl;
        cin>>choice;
    }
    if(choice =1)
    {
    
    String username, password;
    cout<<"select a username"<<endl;
    cin>>username;
    cout<<"select a password"<<endl;
    cin>>password;
    
    
    ofstream file
    file.open("c:\\" + username + ".txt");
    file<<username <<endl <<password;
    file.close();
    
    main();
    {
        else if(choice ==2)
        {
            bool status = IsloggedIn ();
            
            if(!status)
            {
                cout<< "False login "<<endl;
                system("Pause");
                return 0;
            }
            else 
            {
                cout<<"sucessfully login"<<endl;
                system(" Pause");
                return 1;
            }

}
