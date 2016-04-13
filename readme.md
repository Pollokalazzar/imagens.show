import java.text.DateFormat;
import java.util.Date;

import javax.swing.JOptionPane;


public class formatosDeData {

	
	public static void main(String[] args) {
		
		Date agora = new Date();
		
		DateFormat df1,df2,df3,df4,df5;
		String f1,f2,f3,f4,f5;
		
		df1 = DateFormat.getDateInstance();
		df2 = DateFormat.getDateInstance(DateFormat.SHORT);
		df3 = DateFormat.getDateInstance(DateFormat.MEDIUM);
		df4 = DateFormat.getDateInstance(DateFormat.LONG);
		df5 = DateFormat.getDateInstance(DateFormat.FULL);
	
		f1 = df1.format(agora);
		f2 = df2.format(agora);	
		f3 = df3.format(agora);
		f4 = df4.format(agora);	
		f5 = df5.format(agora);       
 	
	
	   JOptionPane.showMessageDialog(null,"Formato Default = " + f1 + "\n Formato short : " + f2 + "\n Formato Medio :" + f3 + "\n formato Longo :" + f4 + "\n formato Full " + f5);
	   
	   
	   System.exit(0);
	
	}  

}



import java.util.Date;

import javax.swing.JOptionPane;


public class utiliza_Date {

	
	public static void main(String[] args) {
		long milissegundosPorDia = 1000*60*60*24;
		
		Date data1 = new Date();
		
		long  tempo1 = data1.getTime();
		
		for (int i = 0; i < 99999999 ; i++);
		
		Date data2 = new Date();
		long tempo2 = data2.getTime();
		
		Date data3 = new Date(data2.getTime() + milissegundosPorDia * 10);
		JOptionPane.showMessageDialog(null, " Milissegundos desde 1970 (1) : " + tempo1 + " \n Milissegundos desde 1970 (2) " + tempo2 + "\n dias : " + tempo2/milissegundosPorDia + "\n Meses: " + tempo2/milissegundosPorDia/30 + "\n anos : " + tempo2/milissegundosPorDia/365 + "\n Data2 :" + data2 + "\n data 3 : " + data3);
		
		System.exit(0);

	}

}

