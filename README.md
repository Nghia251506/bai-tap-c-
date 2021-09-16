#include <iostream>
using namespace std;

class Vec_tor3
{
	private:
		int x,y,z;
	public:
		Vec_tor3()
		{}
		Vec_tor3(int* x, int* y, int* z)
		{
			this-> x, x;
			this-> y, y;
			this-> z, z;
		}
		void input()
		{
			cout<<endl;
			cout<<"Nhap chieu thu 1: ";
			cin>>x;
			cout<<"Nhap chieu thu 2: ";
			cin>>y;
			cout<<"Nhap chieu thu 3: ";
			cin>>z;
		}
		
		void output()
		{
			cout<<"("<<x<<","
					 <<y<<","
					 <<z<<")";
		}
		
		int getx()
		{
			return x;
		}
		
		int gety()
		{
			return y;
		}
		
		int getz()
		{
			return z;
		}
};


int main(int argc, char *argv[])
{
	Vec_tor3 vt[2];
	cout<<"Nhap vao 2 vector: "<<endl;
	for(int i = 1; i <= 2; i++)
	{
		cout<<"Nhap vector thu"<<i+1<<":"<<endl;
		cout<<"--------------------"<<endl;
		vt[i].input();
	}
	cout<<"----------------------"<<endl;
	for(int i = 1; i <= 2; i++)
	{
		cout<<"\nVector thu"<<i+1<<":"<<endl;
		vt[i].output();
	}
	cout<<"\nTong 2 vector ba chieu la: "<<endl;
	vt[1].output();
	cout<<"va";
	vt[2].output();
	cout<<endl;
		cout<<"( "<<vt[1].getx() + vt[2].getx()
			<<", "<<vt[1].gety() + vt[2].gety()
			<<", "<<vt[1].getz() + vt[2].getz()<<")"<<endl;
	return 0;
}
