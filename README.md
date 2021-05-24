# LaundryPalembang

Repo ini adalah kode pemrograman Android Studio (Java) yang mengimplementasikan CRUD dengan MySQL dan Retrofit.

# Database dan Web Service

 - Database : [Download](https://drive.google.com/file/d/1pYUIF_COCYwKte_PNFJbTzISyR52EQXy/view?usp=sharing)
 - Web Services : [Download](https://drive.google.com/file/d/1YxRkgPWDksUD7rkJVqvpadTH6_zyBmMn/view?usp=sharing)

# Video Tutorial

Berikut ini video tutorialnya :

 - Part 1 (Proses Retrieve) : [https://youtu.be/jAZP8ABMeEE](https://www.youtube.com/watch?v=jAZP8ABMeEE&t=0s) 
 - Part 2 (Proses Create) : [https://youtu.be/bcFoCnVhhBI](https://www.youtube.com/watch?v=bcFoCnVhhBI&t=0s) 
 - Part 3 (Proses Delete) : [https://youtu.be/zI-GOXjnE-M](https://www.youtube.com/watch?v=zI-GOXjnE-M&t=0s)
 -  Part 4 (Proses Update)  : [https://youtu.be/zrpGQ8haAqM](https://www.youtube.com/watch?v=zrpGQ8haAqM&t=0s)

# Penyesuaian

Sesuaikan IP Address pada RetroServer.java

    public class RetroServer {
	    private static final String baseURL = "http://10.0.2.2/laundry/";
	    private static Retrofit retro;

	    public static Retrofit konekRetrofit(){
	        if(retro == null){
	            retro = new Retrofit.Builder()
                    .baseUrl(baseURL)
                    .addConverterFactory(GsonConverterFactory.create())
                    .build();
	        }
	        
	        return retro;
	    }
    }

IP di atas adalah IP yang digunakan dengan emulator bawaan Android Studio
