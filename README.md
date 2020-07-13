# counting-no.-of-character-of-string
using hashmap


import java.util.*;
import java.io.*;

public class HelloWorld
{
     public static void main(String []args)
     {
         String str="aabccd";
         char[] ch=str.toCharArray();
         HashMap<Character,Integer> hm=new HashMap<>();
         for(int i=0;i<ch.length;i++)
         {
             if(hm.containsKey(ch[i]))
             {
                 hm.put(ch[i],hm.get(ch[i])+1);
             }
             else
             {
                 hm.put(ch[i],1);
             }
             
         }
         for(Map.Entry entry : hm.entrySet())
         {
             System.out.println(entry.getKey()+" "+entry.getValue());
         }
        
     }
}

