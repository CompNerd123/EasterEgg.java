/*Eugene Vasquez
COMP/ITSE
Easter Egg Generator
Using char and print, output easter egg 
that has characters inside
*/

public class EasterEgg{

    private char chrSign='#';
    
    public EasterEgg(){

        char pcharacter=' ';

    }
    public EasterEgg(char pcharacter){

        this.chrSign=pcharacter;

    }
    public void setSign(char pcharacter){ 

        this.chrSign=pcharacter;

    }
    public char getSign(){

        return chrSign;

    }
    public String toString(){
       
        return ("  __ ")+"\n"+
        (" /"+getSign()+getSign()+"\\")+"\n"+
        ("/"+getSign()+getSign()+getSign()+getSign()+"\\")+"\n"+
        ("|"+getSign()+getSign()+getSign()+getSign()+"|")+"\n"+
        ("\\"+"____"+"/");
    }
    public static void main(String[]args){

        EasterEgg object=new EasterEgg();
        System.out.println(object);
        object.setSign('$');
        System.out.println(object);
        object.setSign('%');
        System.out.println(object);
        EasterEgg object1=new EasterEgg('+');
        System.out.println(object1);
        
    }
}
