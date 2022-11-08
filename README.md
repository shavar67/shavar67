     👋🏾 Construction zone 🚧 | generating new profile.....

```C#
using System;
namespace GithubProfile {
   class Profile {
   class Hello {         
   static void Main(string[] args) {
   Console.WriteLine("New profile coming soon!");}}}
```
    ‼️ Encapsulating profile data
```C#
namespace GitProfileBio { 
    public class User {
        private string name;
        private string title;
        private string interest;
        private string courses;
        
        public string Name { get => name; set => name = value; }
        public string Title { get => title; set => title = value; }
        public string Courses { get => courses; set => courses = value; }
        public string Interest { get => interest; set => interest = value; }
        public User() { Console.WriteLine("Please wait...generating profile bio.\n"); }
        public override string ToString() => 
        "Name: " 
        + Name + "\nTitle: " 
        + Title + "\nInterest: " 
        + Interest 
        + "\ncurrently learning: " 
        + Courses; } }
```
       ⚡️ Generating new profile bio.
```C#
using GitProfileBio;
namespace GithubProfile{
      class Profile  {
        public static void Main(string[] args) {
            var _description = "Shavar.,Software Engineer.,Augmented reality | Artificial Intelligence." +
            ",C# | Ruby | Ruby | Go.";
            var _profile = new Profile();
            _profile.GreetNewVisitors();
            Console.WriteLine(_profile.CreateBio(_description));
            }
        
        public  User CreateBio(string _userData) {
            var _user = new User();
            string[] userDetails = _userData.Split(",");
            for (var i = 0; i < userDetails.Length; i++){
                _user.Name = userDetails[0];
                _user.Title = userDetails[1];
                _user.Interest= userDetails[2];
                _user.Courses= userDetails[3];}
              return _user;}
        
        public void GreetNewVisitors() { 
            string msg = "";
            Console.WriteLine("Welcome to my github profile! have you been here before?");
            string returning = Console.ReadLine();
            if (returning.Equals("yes", StringComparison.OrdinalIgnoreCase)) msg = "\nWelcome back!\n";
            else msg = "Hello!, take a look around!\n";
            Console.WriteLine(msg);}}}
```
     </> Program execution
     Welcome to my github profile! have you been here before?
     no
     Hello!, take a look around!
     Please wait...generating profile bio.
  
  ```C#             
    Name: Shavar.
    Title: Software Engineer.
    Interest: Augmented reality | Artificial Intelligence.
    currently learning: C# | Ruby | Ruby | Go.
 ```

<br/>
<a href="https://github.com/shavar67">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=shavar67&theme=buefy&show_icons=true" />
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=shavar67&theme=buefy&layout=compact" />
</a>
<br/>

