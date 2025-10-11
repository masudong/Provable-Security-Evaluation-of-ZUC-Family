# Supplementary Materials for the ToSC Submission 

For Case-III-1:
1. Use the C program `1.Generate masks m1_p, m2_p` to generate `result.txt`, recording the mask pairs (m1_p, m2_p) that meet the following requirements:
   (1) Record the maximum absolute correlation of S0(m1_p_1 -> k1_1), where MSB(k1_1)!=0;
   (2) The maximum absolute correlation of linear approximations of three parts (modular additions invoved by m2 and m3, S0(m1_p_1 -> k1_1), S1(m1_p_0 -> k1_0)) is less than 2^ -21.1.  

Running this program yields a total of  15503115=2^23.886 masks pairs (m1_p, m2_p).

2. Call the MILP program to calculate the maximum absolute correlation of the two additions and S-boxes such that the absolute correlation < 2^-21.1, and  
   m[0][16] = 1  
   funcADD(M, m[0], m[2], Alpha, Add_s[0])  
   funcADD(M, m[0], m[1], m[3], Add_s[1])  

3. Call the C program to calculate the  absolute correlation of the composite function cor_f().  

---


For Case-III-2:
1. Use the C program  `1.Generate masks m1_p, m2_p` to generate `result.txt`, recording the mask pairs (m1_p, m2_p) that meet the following requirements: 
   (1) Record the maximum bias of S0(m1_p_1 -> k1_1), where MSB(k1_1)!=0; 
   (2) The maximum absolute correlation of linear approximations of three parts (modular additions invoved by m2 and m3, S0(m1_p_1 -> k1_1), S1(m1_p_0 -> k1_0)) is less than 2^ -21.1.
   
Running this program yields a total of  16453063=2^23.972 masks pairs (m1_p, m2_p).

2. Call the MILP program to calculate the maximum absolute correlation of the two additions and S-boxes such that the absolute correlation < 2^-21.1, and   
   funcADD(M, m[0], m[2], Alpha, Add_s[0])  
   funcADD(M, m[0], m[1], m[3], Add_s[1])  

3. Call the C program to calculate the  absolute correlation of the composite function cor_f().  
