## Lab 05
### Develop an android application to display the application name with logo (i.e., YouTube, Facebook, Twitter, TikTok, Snapchat, Telegram, etc.) in Grid View and display their site in another activity when Grid View item clicked.

#### Steps
- Create MainActivity
- Create activity_main.xml
- Add MainActivity to AndroidManifest.xml
- In activity_main
   - Add a GridLayout
   - give grid layout an id
   - make 2 columns
 - In MainActivity
    - Set content view to activity_main
    - Create a private property for GridLayout and assign it by using findViewById
    - Create a Java class called SocialMediaApplication  and put name, imageResourceId and description as its property
    - Create arrayList of SocialMediaApplication in MainACtivity and randomly populate it.
- Create a SocialMediaGridAdapter
   - extends BaseAdapter and implement all four methods
   - Then set this adapter to GridLayout
