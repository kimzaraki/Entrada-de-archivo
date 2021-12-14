#include<fstream>
#include<string>
#include<iostream>

int main(){
	
	std::ifstream inf{"Sample.dat"};
	if(!inf){
		std::cerr<<"uh. oh, sample. dat no puede ser abierto"<<std::endl;
		return 1;
	}
	while(inf){
		std::string strInput;
		inf>>strinInput;
		std::cout<<strinInput<<'\n';
	}
	return 0;
	
}
