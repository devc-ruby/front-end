

# API



**Get close stores**
----
  Returns JSON data about stores in a specific distance.

* **URL:**  `/stores/near`

* **Params:** 
	* distance: number (unit = km)
	* latitude: string
	* longitude: string


* **Method:**  `GET`

* **Success Response:**

  * **Code:** 200
  *  **Content:**
    ```json
    {   
        status : "success",
        data : [
	        {
		        latitude: ,
		        longitude: ,
		        name_store: "The Coffee House",
		        services: "Đồ ăn khuya",		    
		        location: "90 Lê Thúc Hoạch, ... ",
		        image: [
			        {
				        url: "https://lh5.googleusercontent.com/p/AF1QipMJ_hzVAPS6GzJQA3SHLpi1jI2MmJlTp9vJNVe4=w408-h272-k-no",
			        },
    			    {
				        url: "https://lh5.googleusercontent.com/p/AF1QipMJ_hzVAPS6GzJQA3SHLpi1jI2MmJlTp9vJNVe4=w408-h272-k-no",
			        },  
		        ]
	        },
		        review: [
		        {
			        reviewer_name: "Nguyen Tan Dung",
			        reviewer_img: "https://www.google.com/url?sa=t&rct=j&url=https%3A%2F%2Fwww.google.com%2Fmaps%2Fcontrib%2F109380779143355716855%2Freviews%3Fhl%3Dvi&source=maps&ei=iDh2Xd7cDIbpvATk9ar4AQ%3A37&cd=1&usg=AOvVaw1UoOlploPwgOa70gyjs4kU&ved=1t%3A21866%2Cp%3AiDh2Xd7cDIbpvATk9ar4AQ",
			        reviewer_content: "Chuyện là hôm đó team mình hẹn ở TCH(The Coffee House) Sư Vạn Hạnh để ôn bài,khi mình bước vào quán để tới khu vực order thì chị nhân viên có đề",
		        }
	        ]
        ]
	}
	```




**Get Recent Visit Stores**
----
  Returns JSON data about stores that recently visited.

* **URL:**  `/stores/recent`

* **Params:** 
	* amount: number: the number of historical records

* **Method:**  `GET`

* **Success Response:**

  * **Code:** 200
  *  **Content:**
    ```json
    {   
        status : "success",
        data : [
	        {
		        name_store: "The Coffee House",
		        services: "Đồ ăn khuya",		    
		        location: "90 Lê Thúc Hoạch, ... ",
		        payment: "20.000d",
		        image: [
			        {
				        url: "https://lh5.googleusercontent.com/p/AF1QipMJ_hzVAPS6GzJQA3SHLpi1jI2MmJlTp9vJNVe4=w408-h272-k-no",
			        },
    			    {
				        url: "https://lh5.googleusercontent.com/p/AF1QipMJ_hzVAPS6GzJQA3SHLpi1jI2MmJlTp9vJNVe4=w408-h272-k-no",
			        },  
		        ]
	        },
		        
        ]
	}
	```

**Get Feedback  From nearby store **
----
  Returns JSON data about feedback of stores nearby.

* **URL:**  `/feedbacks/near`

* **Params:** 
	* amount: number: the number of historical records

* **Method:**  `GET`

* **Success Response:**

  * **Code:** 200
  *  **Content:**
    ```json
    {   
        status : "success",
        data : {
	        review: [
		        {
			        reviewer_name: "Nguyen Tan Dung",
			        reviewer_avatar: "https://www.google.com/url?sa=t&rct=j&url=https%3A%2F%2Fwww.google.com%2Fmaps%2Fcontrib%2F109380779143355716855%2Freviews%3Fhl%3Dvi&source=maps&ei=iDh2Xd7cDIbpvATk9ar4AQ%3A37&cd=1&usg=AOvVaw1UoOlploPwgOa70gyjs4kU&ved=1t%3A21866%2Cp%3AiDh2Xd7cDIbpvATk9ar4AQ",
			        reviewer_content: "Chuyện là hôm đó team mình hẹn ở TCH(The Coffee House) Sư Vạn Hạnh để ôn bài,khi mình bước vào quán để tới khu vực order thì chị nhân viên có đề",
			        reviewer_img: [
				        {
					        url: "https://lh5.googleusercontent.com/p/AF1QipMJ_hzVAPS6GzJQA3SHLpi1jI2MmJlTp9vJNVe4=w408-h272-k-no",
				        },
	    			    {
					        url: "https://lh5.googleusercontent.com/p/AF1QipMJ_hzVAPS6GzJQA3SHLpi1jI2MmJlTp9vJNVe4=w408-h272-k-no",
				        },  
			        ],
			        store_info: {
				        name_store: "The Coffee House",
				        latitude: "",
					    longtitude: "",
			        }
		        }
	        ]
        }
	}
	```
