# challenge6
// Created on Mon April 6 2020

int left_motor= 0; 
int right_motor= 2; 
int forward= 60;
int backward= -60;
int pause= 1000;

void straight(){
    motor(left_motor,forward);
    motor(right_motor,forward);
	msleep(pause);
    ao();
}
void back(){
    motor(left_motor,backward);
    motor(right_motor,backward);
	msleep(pause);
    ao();
}


int main()
{
	
	int quarantine;
	
	for(quarantine=1; quarantine<=6; quarantine++) {
		straight();
		back();
		printf("quarantine is %d\n", quarantine);
	}
	
return 0;

}
