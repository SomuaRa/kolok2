#include <iostream>
#include <string>

using namespace std;

int main(){
    char a;
    string s; 
    string s1;
    
    cin >> a;
    cin >> s;
    cin >> s1;
    
    for(int i = 0; i < s.length(); ++i) {
        if(s[i] == a) {
            s.insert(i, s1);
            i += s1.length();
        }
    }
    
    cout << s;
    
    system("pause");
    return 0;
}