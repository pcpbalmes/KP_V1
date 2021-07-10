import java.util.Arrays;
import java.util.OptionalInt;


class Scratch {

    public static void main(String[] args) {
        int [] maxPesPreu = {20,15,25,20,10}; //Dividim el pes pel preu per tenir el max pes valor
        int c =45;
        int [] pS =new int[500]; //Com acurar això ?
        int sT=0;
        int count = 0;
        int countSTmp=0;


        if(!sumaTots(maxPesPreu,c)){

            while (count<maxPesPreu.length){
                sT=maxPesPreu[count];
                System.out.print(maxPesPreu[count]+" ");
                for (int i=0;i<maxPesPreu.length;i++){
                    if(i!=count){ //No es el mateix valor
                        if (sT+maxPesPreu[i]<=c){
                            sT+=maxPesPreu[i];
                            pS[countSTmp]+=sT;
                            countSTmp++;
                            System.out.print(maxPesPreu[i]+" ");
                        }
                    }
                }
                count++;
                System.out.println("..............");
            }
        }else{
            System.out.println("Hi caben tots els elements");
        }
    System.out.println(mostra_millor_pes(pS));

    }

    private static OptionalInt mostra_millor_pes(int[] pS) {
        return Arrays.stream(pS).max();
    }

    private static boolean sumaTots(int [] pollastre,int c) {
        int tmp =0;
        for (int i = 0; i < pollastre.length; i++){
            if ((tmp<=c)&&(tmp+pollastre[i]<=c)){
                tmp+=pollastre[i];
            }else{
                return false;
            }
        }
        return true;
    }
}
