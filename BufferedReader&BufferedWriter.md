scanner는 입출력 시 시간이 오래걸림
-> BufferedReader & BufferedWriter 사용

#BufferedReader 사용

BufferedReader bf = new BufferedReader(new InputStreamReader(System.in));
bf.readLine();

String s = bf.readLine();
StringTokenizer st = new StringTokenizer(s);  //한줄씩 입력 받은 후 StringTokenizer로 자름
int a = Integer.parseInt(st.nextToken());
int b = Integer.parseInt(st.nextToken());

bf.close(); //마지막 종료시키기
  
#BufferedWriter 사용
BufferedWriter bw = new BufferedWriter(new OutputStreamWriter(System.out));
bw.write(33 + "\n");  //출력
bw.flush();           //버퍼 비우기
bw.close();           //버퍼 종료

