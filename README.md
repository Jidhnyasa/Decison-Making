# Decison-Making Assignment 1
## Part 2 b) A Bayesian Network in Netica
---
### Random Variables as follows:
1) ProximitySignal(signalyes,signalno)<br>
2) Robotiloc(i11,i12,i13,i14,i21,i22,i23,i24,i31,i32,i33,i34,i41,i42,i43,i44)<br>
3) Robotjloc(j11,j12,j13,j14,j21,j22,j23,j24,j31,j32,j33,j34,j41,j42,j43,j44)<br>
4) Fugitive(Fyes,Fno)<br>
5) Fugitiveloc(f11,f12,f13,f14,f21,f22,f23,f24,f31,f32,f33,f34,f41,f42,f43,f44)<br>
6) FaceRecognition(fryes,frno)<br>
7) Clothes(Cyes,Cno)<br>
------
### Explaination

1) The Robotiloc and Robotjloc location is dependent on proximitysignal, because if the i and j distance is less than or 1        sector the proximitysignal likely to go off is 95% and when it is 2 manhattan distance than the signal likely go off is        80%.
2) The FaceRecognition and Clothes depends on Fugitive, as they help robot i and j to recognize fugitive.
   The probability of facerecognition is 80% and Clothes is 75%.
3) The Robotiloc is parent of FaceRecogniton and Clothes because it recognizes fugitive with the help of facerecognition          software and clothes wearing. 
4) The Fugitiveloc is parent of Fugitive, Robotjloc, FaceRecogniton and Clothes. As it fugitiveloc helps to tell the              probability of fugitive being present.
-----
### Using your BN built in Netica,  answer to the following questions:

i. If a possible fugitive in sector (2,1) is positively recognized using his face but his clothes are not identified, what is    the probability that the fugitive is in (2,1)? How does this probability change when the clothes are also identified? What    is the most probable location(s) of the robot j?<br>
-> The probability that the fugitive is in (2,1) as it is recognized by FaceRecognition is 0.80.
   The probability that the fugitive recognized by clothes is 0.75.
   The most probable location(s) of the robot j is j11(1,1),j22(2,2),j31(3,1).
   
 ii.If robot i’s proximity indicator goes off when it is in location (2,2), what are the probabilities that the fugitive is       located in each of the 16 sectors? What then becomes the most likely location of a fugitive if he is recognized by face       only in (2,3) and by clothes only in (1,2)?<br>
 -> The probabilities that the fugitive is located in each of the 16 sectors is 0.0625
    the most likely location of a fugitive if he is recognized by face only in (2,3) and by clothes only in (1,2) is f23(2,3).
    
 iii.If the proximity indicator goes off when robot i is in sector (2,3) and the fugitive is spotted both by face and clothes      in (2,3) as well,what is the most likely location(s) of the robot j?<br>
 ->  The most likely location(s) of the robot j is j13(1,3),j22(2,2),j24(2,4),j33(3,3)
 
 
