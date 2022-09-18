
import java.awt.FlowLayout;
import java.awt.Font;

import javax.swing.*;  
public class TabbedPaneExample {  
JFrame f;  
TabbedPaneExample(){  
    f=new JFrame();
    JTextArea ta=new JTextArea(200,200); 
    JPanel p1=new JPanel();  
    p1.add(ta);  
    JPanel p2=new JPanel();  
    JPanel p3=new JPanel();  
    JTabbedPane tp=new JTabbedPane();  
    tp.setBounds(50,50,800,800);  
    tp.add("Register",p1); 
	JLabel label=new JLabel("FIRST NAME:",JLabel.LEFT);
	label.setBounds(50, 50, 200, 60);
	p1.add(label);
	p1.setLayout(null);
	JTextField field=new JTextField("enter your first name");
	p1.add(field);
	field.setBounds(180, 50, 200, 30);
	
	JLabel labe1l=new JLabel("LAST NAME:",JLabel.LEFT);	
	labe1l.setBounds(30, 50, 200 , 120);
	p1.add(labe1l);
	p1.setLayout(null);
	JTextField field1=new JTextField("enter your last name");
	p1.add(field1);
	field1.setBounds(180, 90, 250, 70);
	
	JLabel label3=new JLabel("EMAIL:",JLabel.LEFT);	
	label3.setBounds(60, 100, 200 , 200);
	p1.add(label3);
	p1.setLayout(null);
	JTextField field2=new JTextField("enter mail");
	p1.add(field2);
	field2.setBounds(180, 200, 300, 50);
	
	JLabel label4=new JLabel("ROLL NO",JLabel.LEFT);	
	label4.setBounds(60, 180, 200 , 250);
	p1.add(label4);
	p1.setLayout(null);
	JTextField field3=new JTextField("enter roll no");
	p1.add(field3);
	field3.setBounds(180, 270, 350, 60);
	
	JLabel label5=new JLabel("ADDRESS",JLabel.LEFT);	
	label5.setBounds(60, 200, 300 , 350);
	p1.add(label5);
	p1.setLayout(null);
	JTextField field4=new JTextField("enter address");
	p1.add(field4);
	field4.setBounds(180, 350, 300, 70);
	
	
	JLabel label6=new JLabel("GENDER:",JLabel.LEFT);	
	label6.setBounds(60, 300, 350 , 400);
	p1.add(label6);
	p1.setLayout(null);
	JTextField field5=new JTextField("enter gender");
	p1.add(field5);
	field5.setBounds(180, 450, 300, 90);
	JButton b=new JButton("SUBMIT");  
    b.setBounds(50,600,95,30);  
    p1.add(b);  
    JButton b1=new JButton("CANCEL");  
    b1.setBounds(70,600,200,35);  
    p1.add(b1);  
    
    
    tp.add("Login",p2);
    JLabel label9=new JLabel("EMAIL",JLabel.LEFT);	
	label9.setBounds(50, 50, 200, 60);
	p2.add(label9);
	p2.setLayout(null);
	JTextField field9=new JTextField("enter mail");
	p2.add(field9);
	field9.setBounds(180, 50, 200, 30);
	
	JLabel label0=new JLabel("PASSWORD",JLabel.LEFT);
	label0.setBounds(30, 50, 200 , 120);
	p2.add(label0);
	p2.setLayout(null);
	JTextField field0=new JTextField("enter password");
	p2.add(field0);
	field0.setBounds(180, 90, 250, 70);
	JButton b2=new JButton("LOGIN");  
    b2.setBounds(50,200,95,30);  
    p2.add(b2); 
    
    tp.add("Search",p3); 
    JLabel label11=new JLabel("NAME",JLabel.LEFT);
	label11.setBounds(30, 50, 200 , 120);
	p3.add(label11);
	p3.setLayout(null);
	JTextField field11=new JTextField("ENTER YOUR NAME HERE");
	field11.setBounds(180, 90, 250, 70);
	p3.add(field11);
	JButton b3=new JButton("SEARCH");  
    b3.setBounds(50,200,95,30);  
    p3.add(b3); 
    f.add(tp);  
    f.setSize(800,800);  
    f.setLayout(null);  
    f.setVisible(true);  
}  
public static void main(String[] args) {  
    new TabbedPaneExample();  
}}  
