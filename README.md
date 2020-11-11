# blowfish-algorithm
/// Real quick, anything i am copy/pastn', it looks like they are needed in code than personalizing
implementation of the blowfish crytographic algorithm
<iostream>
<cmath>
<random>  
  
// generate subkeys

 subkey [] = rand(8) + 1;


P[0] = {"ooga booga text"};
etc...

//intializing

String P[]= {"smaller version"}

// to store 2^32(for addition modulo 2^32). 
    long modVal = 1;

  // to convert hexadecimal to binary. 
    private String hexToBin(String plainText) 
    { 
        String binary = ""; 
        Long num; 
        String binary4B; 
        int n = plainText.length(); 
        for (int i = 0; i < n; i++) { 
  
            num = Long.parseUnsignedLong( 
                plainText.charAt(i) + "", 16); 
            binary4B = Long.toBinaryString(num); 
  
            // each value in hexadecimal is 4 bits in binary. 
            binary4B = "0000" + binary4B; 
  
            binary4B = binary4B.substring(binary4B.length() - 4); 
            binary += binary4B; 
        } 
        return binary; 
    }
    
    
     // convert from binary to hexadecimal. 
    private String binToHex(String plainText) 
    { 
  
        long num = Long.parseUnsignedLong(plainText, 2); 
        String hexa = Long.toHexString(num); 
        while (hexa.length() < (plainText.length() / 4)) 
  
            // maintain output length same length 
            // as input by appending leading zeroes. 
            hexa = "0" + hexa; 
  
        return hexa; 
    } 
