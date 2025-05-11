#include<iostream>
#include<string>
#include<cmath>
using namespace std;
int main()
{
	int acc_1=11111,acc_2=22222,acc_3=33333;
	int pin_1=1111, pin_2=2222, pin_3=3333;
	int acc_1_cash=5000,acc_2_cash=10000,acc_3_cash=15000;
	int a,b,c,d,e;
	cout<<"\t\t Welcome to Meezan Banking System"<<endl;
	cout<<"Enter you Account Nmuber : ";
	cin>>a;
	if(a==acc_1)
	{
		cout<<"Your Account Number is matched: "<<endl;
		cout<<"Enter Your PIN Code"<<endl;
		cin>>b;
		if(b==pin_1)
		{
			cout<<"You are verified "<<endl;
			system("cls");
			cout<<"Press \n 1-Check Balance \n 2-Deposit \n 3-Withdraw \n 4-Transfer "<<endl;
		    cin>>c;
		switch(c)
		{
		
		    case 1:
		    {
		    	cout<<acc_1_cash<<endl;
			break;
			}
		    break;
			case 2:
		    {
		    	cout<<"How much Money You want to deposit"<<endl;
		    	cin>>d;
		    	acc_1_cash=acc_1_cash+d;
		    				system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_1_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
			break;
			}
			case 3:
			{
				cout <<"How much Money you want to withdraw"<<endl;
				cin>> d;
				if(d<acc_1_cash)
				{
					acc_1_cash=acc_1_cash-d;
							system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_1_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
				}
				else if(acc_1_cash<d)
				{
					acc_1_cash=d-acc_1_cash;
							system("cls");
			                cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_1_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
				}
			}break;
			case 4:
			{
				cout<<"In which account you want to transfer the money"<<endl;
				cout<<"Press \n 1-Account_2 \n 2-Account-3"<<endl;
				cin>>d;
				switch(d)
				{
				case 1 :
					{
						cout<<"You select the Account 2"<<endl;
						cout<<"How much money you want to transfer"<<endl;
						start :
						cin>>e;
						acc_2_cash=acc_2_cash+e;
						if(e<=acc_1_cash)
						{
							acc_1_cash=acc_1_cash-e;
							system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_1_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
						}
						else
						{
							cout<<"Enter the Right amount"<<endl;
						    goto start;
						}
					}break;
				
				case 2 :
					{
						cout<<"You select the Account 3"<<endl;
						cout<<"How much money you want to transfer"<<endl;
						again :
						cin>>e;
						acc_3_cash=acc_3_cash+e;
						if(e<=acc_1_cash)
						{
							acc_1_cash=acc_1_cash-e;
							system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_1_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
						}
						else
						{
							cout<<"Enter the Right amount"<<endl;
						    goto again;
						}
					}break;	
			    }
					
			}break;
			}
		}
		else
		{
			cout<<"Incorect Pin"<<endl;
		}
	}
	else if(a==acc_2)
	{
		cout<<"Your account is matched "<<endl;
		cout<<"Enter your PIN Code"<<endl;
		cin>>b;
		if(b==pin_2)
		{
			cout<<"You are verified "<<endl;
		system("cls");
			cout<<"Press \n 1-Check Balance \n 2-Deposit \n 3-Withdraw \n 4-Transfer "<<endl;
		    cin>>c;
		switch(c)
		{		
		    case 1:
		    {
		    	cout<<acc_2_cash<<endl;
			break;
			}
		    break;
			case 2:
		    {
		    	cout<<"How much Money You want to deposit"<<endl;
		    	cin>>d;
		    	acc_2_cash=acc_2_cash+d;
		    	system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_2_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
			break;
			}
			case 3:
			{
				cout <<"How much Money you want to withdraw"<<endl;
				cin>> d;
				if(d<acc_2_cash)
				{
					acc_2_cash=acc_2_cash-d;
					system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_2_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
				}
				else if(acc_2_cash<d)
				{
					acc_2_cash=d-acc_2_cash;
					system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_2_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
				}
			}break;
			case 4:
			{
				cout<<"In which account you want to transfer the money"<<endl;
				cout<<"Press \n 1-Account_1 \n 2-Account-3"<<endl;
				cin>>d;
				switch(d)
				{
				case 1 :
					{
						cout<<"You select the Account 1"<<endl;
						cout<<"How much money you want to transfer"<<endl;
						first :
						cin>>e;
						acc_1_cash=acc_1_cash+e;
						if(e<=acc_2_cash)
						{
							acc_2_cash=acc_2_cash-e;
							
							system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_2_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
						}
						else
						{
							cout<<"Enter the Right amount"<<endl;
						    goto first;
						}
					}break;
				
				case 2 :
					{
						cout<<"You select the Account 3"<<endl;
						cout<<"How much money you want to transfer"<<endl;
						second :
						cin>>e;
						acc_3_cash=acc_3_cash+e;
						if(e<=acc_2_cash)
						{
							acc_2_cash=acc_2_cash-e;
							system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_2_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
						}
						else
						{
							cout<<"Enter the Right amount"<<endl;
						    goto second;
						}
					}break;	
			    }
					
			}break;
		}
	}
		
		else
		{
			cout<<"Incorect Pin"<<endl;			
		}
	
	}
	else if(a==acc_3)
	{
		cout<<"Your account is matched "<<endl;
		cout<<"Enter your PIN Code"<<endl;
		cin>>b;
		if(b==pin_3)
		{
			cout<<"You are verified "<<endl;
		system("cls");
			cout<<"Press \n 1-Check Balance \n 2-Deposit \n 3-Withdraw \n 4-Transfer "<<endl;
		    cin>>c;
		switch(c)
		{
		
		    case 1:
		    {
		    	cout<<acc_3_cash<<endl;
			break;
			}
		    break;
			case 2:
		    {
		    	cout<<"How much Money You want to deposit"<<endl;
		    	cin>>d;
		    	acc_3_cash=acc_3_cash+d;
		    	system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_3_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
							cout<<"\t*****************************"<<endl;
			break;
			}
			case 3:
			{
				cout <<"How much Money you want to withdraw"<<endl;
				cin>> d;
				if(d<acc_3_cash)
				{
					acc_3_cash=acc_3_cash-d;
					system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_3_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
							cout<<"\t*****************************"<<endl;
				}
				else if(acc_3_cash<d)
				{
					acc_3_cash=d-acc_3_cash;
					system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_3_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
							cout<<"\t*****************************"<<endl;
				}
			}break;
			case 4:
			{
				cout<<"In which account you want to transfer the money"<<endl;
				cout<<"Press \n 1-Account_1 \n 2-Account-2"<<endl;
				cin>>d;
				switch(d)
				{
				case 1 :
					{
						cout<<"You select the Account 1"<<endl;
						cout<<"How much money you want to transfer"<<endl;
						third :
						cin>>e;
						acc_1_cash=acc_1_cash+e;
						if(e<=acc_3_cash)
						{
							acc_3_cash=acc_3_cash-e;
							system("cls");
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_3_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
							cout<<"\t*****************************"<<endl;
						}
						else
						{
							cout<<"Enter the Right amount"<<endl;
						    goto third;
						}
					}break;
				case 2 :
					{
						cout<<"You select the Account 2"<<endl;
						cout<<"How much money you want to transfer"<<endl;
						fourth :
						cin>>e;
						acc_2_cash=acc_2_cash+e;
						if(e<=acc_3_cash)
						{
							system("cls");
							acc_3_cash=acc_3_cash-e;
							cout<<"\t Reciept "<<endl;
							cout<<"Now your Remaining balance is : "<<acc_3_cash<<endl;
						    cout<<"Charges = 0.00"<<endl;
							cout<<"Thanks for using Meezan ATM"<<endl;
						    cout<<"\t Save Money : Save life  "<<endl;
						    cout<<"\t*****************************"<<endl;
						}
						else
						{
							cout<<"Enter the Right amount"<<endl;
						    goto fourth;
						}
					}break;	
			    }
			}break;
		}
	}		
		else
		{
			cout<<"Incorect Pin"<<endl;			
		}
		}
		else
	{
		cout<<"Next Please."<<endl;
	}
	return 0;
}
