package codingTest;

import java.io.BufferedReader;
import java.io.BufferedWriter;
import java.io.IOException;
import java.io.InputStreamReader;
import java.io.OutputStreamWriter;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.List;

//2024.8.31 Programmers codingTest 
//solution 문자열의 앞에 n글자
//solution01 문자열 잘라서 정렬하기
/* 
 * solution 문제설명
 * 문자열 my_string과 정수 n이 매개변수로 주어질 때, 
 * my_string의 앞의 n글자로 이루어진 문자열을 return 하는 
 * solution 함수를 작성해 주세요.
 * -------------------------------------
 * solution01 문제설명
 * 문자열 myString이 주어집니다. "x"를 기준으로 해당 문자열을 잘라내 배열을 만든 후 사전순으로 정렬한 배열을
 *  return 하는 solution 함수를 완성해 주세요.
 *  단, 빈 문자열은 반환할 배열에 넣지 않습니다.
 */

public class Programmers02 {

	public static void main(String[] args) throws IOException {
		
		BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
		BufferedWriter bw = new BufferedWriter(new OutputStreamWriter(System.out));
		
		String inputStr = br.readLine();
		//int n = Integer.parseInt(br.readLine());
		
		//bw.write(solution(inputStr,n));
		bw.write(Arrays.toString(solution01(inputStr)));
		bw.flush();
		bw.close();
		

	}
	
	    public static String solution(String my_string, int n) {
	        
	        String rslt = my_string.substring(0,n);
	        
	        return rslt;
	    }
	    
	   
	    public static String[] solution01(String myString) {
	            
            String[] rslt = myString.split("x+");
            //x+ : x가 하나이상 연속인경우 연속된숫자 기준으로 split
            
            List<String> arrList = new ArrayList<>();
            
            for(String str : rslt) {
            	if(!str.isEmpty()) {
            		arrList.add(str);
            	}
            }
            // 배열 rslt 기준으로 for문을 돌릴때 리스트가 비어있지않으면 새로운 배열에 집어넣음
            
            String[] rsltArray = arrList.toArray(new String[0]);
            // 리스트를 배열로 변경
            
            Arrays.sort(rsltArray);        
            // 배열을 순차로 나열함
            
            return rsltArray;
            
            
        }
	    
/*	   
 * 
 *  용현 코드
 *  
 *  public static String[] solution(String mystring) {
	        String[] arr = mystring.split("x");
	        int n = 0;

	        for (int i = 0; i < arr.length; i++){
	            if (!arr[i].equals("")){
	                arr[n] = arr[i];
	                n++;
	            }
	        }
	 반례 : dxccxbbbxxxaaaa
	 n을 정의하고 새 배열 result 를 만든 이유는 :
	 arr.length 를 그대로 result 배열의 크기로 가져오게 되면
	 arr.length = 5 일때 result배열의 크기도 5로 가져와지는데
	 실제 저장은 다음과 같이: [aaaa, bbb, cc, d, ] 마지막 값에 아무것도 안들어간 배열이 생성되어
	 arr[i] 가 빈값이 아닌경우의 크기를 가져오려고 n 을 저장해서 result[n] 으로 만들어줌
	        String[] result = new String[n];
	        for (int i = 0; i < n; i++){
	            if (!arr[i].isEmpty()){
	                result[i] = arr[i];
	            }
	        }
	        Arrays.sort(result);
	        return result;
	    }
	    public static String[] solution(String mystring) {
	        List<String> result = new ArrayList<>();
	
	        StringTokenizer st = new StringTokenizer(mystring, "x");
	
	        while (st.hasMoreTokens()){
	            result.add(st.nextToken());
	        }
	
	        String[] rst = result.toArray(new String[0]);
	        Arrays.sort(rst);
	        System.out.println(Arrays.toString(rst));
	
	        return rst;
	
	    }

	}
	*/

	}


