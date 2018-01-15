# Return-a-Maximum-value-of-an-Array-of-5-places-in-java
How to return a Maximum value of an Array of 5 places in java

package H.A;

import java.util.Scanner;

public class hhi {
public static int akrab(int [][]hesha){
	int max=0;
	int average;
	for(int i=0;i<5;i++){
		average=0;
		for(int j=1;j<3;j++){
			average=average+hesha[i][j];
			if(max<average){
				max=average;
			}
		}
	}
	return max;
}
	public static void main(String[] args) {
		int[][]hesha=new int[5][3];
		Scanner input = new Scanner(System.in);
		for(int i=0;i<5;i++){
			for(int j=0;j<3;j++){
				hesha[i][j]= input.nextInt();
			}
		}
		System.out.println(akrab(hesha));
	}
}
