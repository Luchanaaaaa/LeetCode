20. Valid Parentheses 
```java
class Solution {
    public boolean isValid(String s) {
        if(s.length()%2!=0) return false;
        Stack<Character> st = new Stack<>();
        // for(char s : )
        // if()
        for(int i = 0; i < s.length(); i ++){
            Character word = s.charAt(i);
            if(word == '{' ||word == '(' || word == '[' ){
                st.push(word);
            }else{
                if(st.isEmpty()) return false;
                Character word2 = st.pop();
                 if((word=='}' && word2!='{') || (word==']' && word2 != '[') || (word==')' && word2 != '(')){  
                     return false;
                     
                 }
            }
        }
        if(st.isEmpty()) return true;
        else return false;


    }
} 
```
