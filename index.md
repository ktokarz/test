About
=====

aewwer

Features
--------

  * sdf
  * qwe
  * fdgge


Requirements
------------

```java
public class ReadByteFromFile {
 
  public static void main(String[] args) {
   
    String strFilePath = "C://FileIO//readByte.txt";
   
    try
    {
      //create FileInputStream object
      FileInputStream fin = new FileInputStream(strFilePath);
     
      /*
       * To create DataInputStream object, use
       * DataInputStream(InputStream in) constructor.
       */
     
       DataInputStream din = new DataInputStream(fin);
     
       /*
        * To read a Java byte primitive from file, use
        * byte readByte() method of Java DataInputStream class.
        */
       
        byte b = din.readByte();
       
        System.out.println("byte : " + b);
       
        /*
         * To close DataInputStream, use
         * void close() method.
         */
         din.close();
       
    }
    catch(FileNotFoundException fe)
    {
      System.out.println("FileNotFoundException : " + fe);
    }
    catch(IOException ioe)
    {
      System.out.println("IOException : " + ioe);
    }
  }
}
```
