# AdventOfCyber2023
Explanation of CTF Advent of Cyber2023 tryhackme solutions   ***    Explanation and solution rights OLEVER@linuxqueenn12
   
   
       *day 3* (OSINT)
        instagram @linuxqueenn
 is gathering and analysing publicly available data for intelligence purposes, which includes information collected from the internet, mass media, specialist journals and research, photos, and geospatial information
تقوم OSINT بجمع وتحليل البيانات المتاحة للجمهور لأغراض استخبارية ، والتي تشمل المعلومات التي تم جمعها من الإنترنت ووسائل الإعلام والمجلات المتخصصة والبحوث والصور والمعلومات الجغرافية المكانية
----------------------------------------------------------------------------OSINT Techniques
Google Dorks Google Dorking involves using specialist search terms and advanced search operators to find results that are not usually displayed using regular search 
----------------------------------------------------------------------------
                            * google dorking *  
1- inurl: Searches for a specified text in all indexed URLsللبحث عن نص محدد في كافة عناوين URL  سيجلب جميع عناوين URL التي تحتوي على كلمة "hacking"

2- filetype: Searches for specified file extensions filetype: pdf "hacking" سيجلب جميع ملفات pdf التي تحتوي على كلمة "hacking"

3- site: Searches all the indexed URLs for the specified domain يبحث في جميع عناوين URL المفهرسة للمجال المحدد سيقوم موقع tryhackme.com بإحضار جميع عناوين URL المفهرسة من tryhackme.com

4- cache: Get the latest cached version by the Google search engine احصل على أحدث نسخة مخبأة بواسطة محرك بحث Google. على سبيل المثال ، ذاكرة التخزين المؤقت: tryhackme.com

5- site:github.com "DB_PASSWORD" to search only in github.com and look for the string DB_PASSWORD possible
---------------------------------------------------------------------------- 
                                * whois *  
WHOIS database stores public domain information such as registrant (domain owner), administrative, billing and technical contacts in a centralised database. The database is publicly available for people to search against any domain and enables acquiring Personal Identifiable Informationتخزن قاعدة بيانات WHOISمعلومات المجال العام مثل المسجل (مالك المجال)وجهات الاتصال الإدارية والفوترة والتقنية في قاعدة بيانات مركزية قاعدة البيانات متاحة للجمهور للأشخاص للبحث في أي مجال وتمكن من الحصول على معلومات التعريف الشخصية                              ----------------------------------------------------------------------------
                               * robots.txt *
Since the file is publicly accessible, it doesn't mean anyone can edit or modify it. You can access robots.txt by simply appending robots.txt at the end of the website URL. For example, in the case of Google, we can access the robots.txt file by clicking this URL نظرًا لأن الملف متاح للجميع ، فهذا لا يعني أنه يمكن لأي شخص تعديله أو تعديله. يمكنك الوصول إلى ملف robots.txt ببساطة عن طريق إلحاق ملف robots.txt في نهاية عنوان URL لموقع الويب. على سبيل المثال ، في حالة Google ، يمكننا الوصول إلى ملف robots.txt بالنقر فوق عنوان URL هذا
----------------------------------------------------------------------------                                * answers *
1- What is the name of the Registrar for the domain santagift.shop? write whois santagift.shop(Namecheap, Inc)

2- Find the website's source code (repository) on github.com and open the file containing sensitive credentials. Can you find the flag?open santagift.shop on github you can see flag on config.php {THM_OSINT_WORKS}

3- What is the name of the file containing passwords?open the same repository and copy the name (config.php)

4- What is the name of the QA server associated with the website?in the last page(qa.santagift.shop)

5- What is the DB_PASSWORD that is being reused between the QA and PROD environments? (S@nta2022) you can see it in the config.php 
----------------------------------------------------------------------------
                        instagram @linuxqueenn
                        
                       
