class StudentCard {  
  int id;   //学籍番号  
  String name;  //氏名    
  
  StudentCard() {  
    System.out.println("引数のないコンストラクタが実行されました");  
    this.id = 0;  
    this.name = "未定";  
  }    
  StudentCard(String name) {  
    System.out.println("引数が１つのコンストラクタが実行されました");  
    this.id = 0;  
    this.name = name;  
  }  
  StudentCard(int id, String name) {  
    System.out.println("引数が２つのコンストラクタが実行されました");  
    this.id = id;  
    this.name = name;  
  }    
}

public class ConstructorOverloadExample {  
  public static void main(String[] args) {  
    StudentCard a = new StudentCard();  
    System.out.println("aのidの値は" + a.id);  
    System.out.println("aのnameの値は" + a.name);  
    
    StudentCard b = new StudentCard("鈴木太郎");  
    System.out.println("bのidの値は" + b.id);  
    System.out.println("bのnameの値は" + b.name);  
    
    StudentCard c = new StudentCard(1235, "佐藤花子");  
    System.out.println("cのidの値は" + c.id);  
    System.out.println("cのnameの値は" + c.name);  
  }
}

実行結果  
引数のないコンストラクタが実行されました
aのidの値は0
aのnameの値は未定
引数が１つのコンストラクタが実行されました
bのidの値は0
bのnameの値は鈴木太郎
引数が２つのコンストラクタが実行されました
cのidの値は1235
cのnameの値は佐藤花子
