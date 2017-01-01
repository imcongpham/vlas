# vlas
VLAS (A Vietnamese Question and Answering System) is built based on Java. A system that gives you directly answers using Lucence and vnTokenizer.

Hướng dẫn setup hệ thống hỏi đáp VLAS.TXT
------------------------------------------------------------------------------------------------------------------------------------------------------------
Hệ thống được xây dựng trên eclipse Release 4.4.0, June 5, 2014.
Yêu cầu hệ thống:

	1. Java version 1.8.0_45
	
	2. Tomcat Server v8.0 (https://tomcat.apache.org/download-80.cgi)
	
	3. Mavern

Hướng dẫn setup hệ thống:	

	1. Tải và cài đặt Tomcat Server v8.0 (https://tomcat.apache.org/download-80.cgi)
	
	2. Chép file thực thi vlas.war vào thư mục webapp của Apache Tomcat
	
	3. Thư mục resources chứa các file index, token, tập từ đồng nghĩa... phải bỏ trong đường dẫn "C:\User\<Tên User của bạn>\"
	
	4. Trong thư mục resources/models: cấu hình lại file tokenizer.properties chứa đường dẫn đến các thư mục con của token:
	
		lexiconDFA=C:\\Users\\<Tên User của bạn>\\resources\\automata\\dfaLexicon.xml
		
		externalLexicon=C:\\Users\\<Tên User của bạn>\\resources\\automata\\externalLexicon.xml
		
		normalizationRules=C:\\Users\\<Tên User của bạn>\\resources\\normalization\\rules.txt
		
		lexers=C:\\Users\\<Tên User của bạn>\\resources\\lexers\\lexers.xml
		
		unigramModel=C:\\Users\\<Tên User của bạn>\\resources\\bigram\\unigram.xml
		
		bigramModel=C:\\Users\\<Tên User của bạn>\\resources\\bigram\\bigram.xml
		
		namedEntityPrefix=C:\\Users\\<Tên User của bạn>\\resources\\prefix\\namedEntityPrefix.xml
		
	5. Run Tomcat Server
	
	6. URL: localhost:8080/vlas, hệ thống sẵn sàng thực thi
	
------------------------------------------------------------------------------------------------------------------------------------------------------------
Thông tin liên lạc tác giả:

Khoa học tự nhiên

Khoa Công Nghệ Thông Tin
Bộ Môn Hệ Thống Thông Tin

Họ tên: Phạm Thành Công
Email cá nhân: ptcong666@gmail.com

------------------------------------------------------------------------------------------------------------------------------------------------------------
