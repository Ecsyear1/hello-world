# hello-world
  //crack a 5 characters by bruteforce
  // Assume an infinite amount of trials allowed
#include <iostream>
#include <string>
#include <iomanip>
using namespace std;
  int ascii; ascii=256;
 
string brute_force(string pword) {
  
  for (int char1=0; char1<ascii; char1++) {
   for (int char2=0; char2<ascii; char2++) {
    for (int char3=0; char3<ascii; char3++) {
     for (int char4=0; char4<ascii; char4++){
     for (int char5=0;char5<ascii;char5++)//digit to char
     //concatenation
      string attempt = string()+(char)char1+(char)char2+(char)char3+(char)char4+ (char)char5;
      if (attempt==pword) return attempt;
      }
     }
    }
   }
  }
  throw "not found";
  return o;
