**LEETCODE-344**



class Solution {

&#x20;   public void reverseString(char\[] s) {

&#x20;       int l=0;

&#x20;       int r=s.length-1;

&#x20;       while(l<r){

&#x20;           char t=s\[l];

&#x20;           s\[l]=s\[r];

&#x20;           s\[r]=t;

&#x20;           l++;

&#x20;           r--;



&#x20;       }



&#x20;   }

}



**LEETCODE-876**



class Solution {

&#x20;   public ListNode middleNode(ListNode head) {

&#x20;       ListNode slow=head;

&#x20;       ListNode fast=head;

&#x20;       while(fast!=null \&\& fast.next!=null){

&#x20;           slow=slow.next;

&#x20;           fast=fast.next.next;

&#x20;       }

&#x20;       return slow;

&#x20;   }

}



**LEETCODE-387**



class Solution {

&#x20;   public int firstUniqChar(String s) {

&#x20;       for(int i=0;i<s.length();i++){

&#x20;           char ch=s.charAt(i);

&#x20;           if(s.indexOf(ch)==s.lastIndexOf(ch)){

&#x20;               return i;

&#x20;           }

&#x20;       }

&#x20;       return -1;

&#x20;   }

}



**LEETCODE-205**



class Solution {

&#x20;   public boolean isIsomorphic(String s, String t) {

&#x20;       for(int i=0;i<s.length();i++){

&#x20;           char c=s.charAt(i);

&#x20;           char d=t.charAt(i);

&#x20;            if(s.indexOf(c)!=t.indexOf(d)){

&#x20;               return false;

&#x20;            }

&#x20;       }

&#x20;       return true;

&#x20;   }

}



**LEETCODE-28**



class Solution {

&#x20;   public int strStr(String haystack, String needle) {

&#x20;       return haystack.indexOf(needle);

&#x20;   }

}



**LEETCODE-1832**



class Solution {

&#x20;   public boolean checkIfPangram(String sentence) {

&#x20;       for(char i='a';i<='z';i++){

&#x20;           if(sentence.indexOf(i)==-1){

&#x20;               return false;

&#x20;           }

&#x20;       }

&#x20;       return true;

&#x20;   }

}



**LEETCODE-242**



class Solution {

&#x20;   public boolean isAnagram(String s, String t) {

&#x20;       char a\[]=s.toCharArray();

&#x20;       char b\[]=t.toCharArray();

&#x20;       Arrays.sort(a);

&#x20;       Arrays.sort(b);

&#x20;       return Arrays.equals(a,b);



&#x20;   }

}



**LEETCODE-1108**



class Solution {

&#x20;   public String defangIPaddr(String address) {

&#x20;       return address.replace(".","\[.]");

&#x20;   }

}









