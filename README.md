
/**
 * Array App
 *
 * @author Joy Posma Abednego Gultom
 * @NRP    5025201103 
 */
public class ArrayApp
{
   public static void main(String[]args)
   {
       long[]arr;//reference to array
       arr= new long [100];//make array
       int nelemen = 0;//number of items
       int j;//loop counter
       long searchkey;//key of item to search
       
       arr[0]=77;// insert 10 items
       arr[1]=21;
       arr[2]=34;
       arr[3]=56;
       arr[4]=89;
       arr[5]=41;
       arr[6]=99;
       arr[7]=68;
       arr[8]=00;
       arr[9]=17;
       nelemen=10;//total 10 items in array
       for(j=0;j<nelemen;j++)//display items
       System.out.print(arr[j] + "\n" );
       System.out.print("");
       
       //search key 99
       searchkey=99;
       for(j=0;j<nelemen;j++)
       if(arr[j]==searchkey)
       break;
       if(j==nelemen)
       System.out.print("Tidak Ditemukan "+searchkey);
       else
       System.out.print("Ditemukan " +searchkey);
       
       //delete key 00
       searchkey=00;
       for(j=0;j<nelemen;j++)
       if(arr[j]==searchkey)
       break;
       for(int k=j;k<nelemen;k++)
       arr[k]=arr[k+1];
       nelemen--;
       for(j=0;j<nelemen;j++)
       System.out.print(" \n"+arr[j]);
       
    }
}

