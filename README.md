#include <iostream>
#include <cstdlib>
#include <cctype> 


using namespace std;
int main() {
	char a[20],b[20],c[20];
	int j=0,idx=0;
	cout<<"Enter word to check a Palindrome: ";
	cin.getline(a,20);
	for (int i=0;i<strlen(a);i++){
			if(isalpha(a[i])!=0){
				c[idx]=tolower(a[i]);
				idx++;
			}
			
		}
		c[idx]='\0';
		for(int i=strlen(c)-1;i>=0;i--){
				b[j]=c[i];
				j++;
			}
			b[strlen(c)]='\0';
			if(strcmp(c,b)==0){
				cout<< "This is a palindrome." <<endl;
			}else{
				cout<< "this is not a palindrome."<<endl;
			}
			 return 0;

	
	
	
}
