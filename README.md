public class JavaBasics {
    public static int Btod(int bino){
        int pow = 0;
        int decno = 0;

        while ( bino > 0){
            int ld = bino % 10 ;
            decno = decno + (int)(ld * Math.pow(2,pow))  ;

            pow++;
            bino = bino /10 ;

        }return decno;
    }
    public static void main (String args[]){
        int bintodi = Btod(1011);
        System.out.println(bintodi);
    }
}
