<p align="center">
  <a href="https://stackoverflow.com/users/7602110/">
    <img src="https://cdn.svgporn.com/logos/stackoverflow.svg">  
    <img src="https://stackoverflow.com/users/flair/7602110.png" width="180" height="50">
   </a>
</p>

> Repo to put my stuff from stackoverflow, not accepting pull requests! [@stackoverflow/abranhe](https://stackoverflow.com/users/7602110/carlos-abraham)

# Answers


1. [46476470](46476470) - Can't create project on Netbeans 8.2
1. [4346786](4346786) - Create Test Class in IntelliJ
1. [901712](901712) - How to check whether a checkbox is checked in jQuery?
1. [34820275](34820275) - Count how many times elements in an array are repeated
1. [842059](842059) - Is there a portable way to get the current username in Python?
1. [40424298](40424298) - Find OS username in NodeJS
1. [19712903](19712903) - Reverse Contents in Array
1. [16151018](16151018) - npm throws error without sudo
1. [39927452](39927452) - Recursively print all permutations of a string (Javascript)
1. [19053707](19053707) - Converting Snake Case to Lower Camel Case (lowerCamelCase)
1. [32621988](32621988) - Electron: jQuery is not defined
1. [4302027](4302027) - how to open a url in python
1. [37672694](37672694) - Can I submit a pull request from GitLab.com to GitHub?
1. [743806](743806) - How to split a string into a list?
1. [48290146](48290146) - Read a text file in windows directory outside eclipse project
1. [28226229](28226229) - Bash: Looping through dates
1. [48027543](48027543) - CSS/JS- Split image in two animation
1. [51372391](51372391) - Github as content management
1. [40407124](40407124) - Android Studio 2.2.2 : Tools > Android menu is missing in Mac OS X
1. [48507685](48507685) - GitHub public link format for accessing my website
1. [47900175](47900175) - Git Bash still pushing with previous username
1. [47971759](47971759) - GitHub pages index page url


Generate everything from the API: ([api.stackexchange.com/docs](https://api.stackexchange.com/docs))

**GET** `
https://api.stackexchange.com/2.2/users/7602110/answers?fromdate=1451606400&todate=1553040000&order=asc&sort=activity&site=stackoverflow`

Example response: 

```json
{
  "items": [
    {
      "owner": {
        "reputation": 606,
        "user_id": 7602110,
        "user_type": "registered",
        "profile_image": "https://i.stack.imgur.com/8t6DY.png?s=128&g=1",
        "display_name": "Carlos Abraham",
        "link": "https://stackoverflow.com/users/7602110/carlos-abraham"
      },
      "is_accepted": false,
      "score": 0,
      "last_activity_date": 1551384838,
      "last_edit_date": 1551384838,
      "creation_date": 1551373139,
      "answer_id": 54930715,
      "question_id": 24989694
    },
    {
      "owner": {
        "reputation": 606,
        "user_id": 7602110,
        "user_type": "registered",
        "profile_image": "https://i.stack.imgur.com/8t6DY.png?s=128&g=1",
        "display_name": "Carlos Abraham",
        "link": "https://stackoverflow.com/users/7602110/carlos-abraham"
      },
      "is_accepted": false,
      "score": 0,
      "last_activity_date": 1552680439,
      "last_edit_date": 1552680439,
      "creation_date": 1552679767,
      "answer_id": 55189850,
      "question_id": 48166731
    },
    {
      "owner": {
        "reputation": 606,
        "user_id": 7602110,
        "user_type": "registered",
        "profile_image": "https://i.stack.imgur.com/8t6DY.png?s=128&g=1",
        "display_name": "Carlos Abraham",
        "link": "https://stackoverflow.com/users/7602110/carlos-abraham"
      },
      "is_accepted": false,
      "score": 0,
      "last_activity_date": 1553022907,
      "last_edit_date": 1553022907,
      "creation_date": 1553022025,
      "answer_id": 55248289,
      "question_id": 34648738
    }
  ],
  "has_more": false,
  "quota_max": 10000,
  "quota_remaining": 9989
}
```

To Question title

**GET** `https://api.stackexchange.com/2.2/questions/48507685?order=desc&sort=activity&site=stackoverflow`

Example response: 

```json
{
  "items": [
    {
      "tags": [
        "github",
        "github-pages"
      ],
      "owner": {
        "reputation": 8,
        "user_id": 9285118,
        "user_type": "registered",
        "profile_image": "https://www.gravatar.com/avatar/fed85e4f64f09c526ddc868c22b02d72?s=128&d=identicon&r=PG&f=1",
        "display_name": "MasterArchivist",
        "link": "https://stackoverflow.com/users/9285118/masterarchivist"
      },
      "is_answered": true,
      "view_count": 81,
      "accepted_answer_id": 48507799,
      "answer_count": 2,
      "score": 1,
      "last_activity_date": 1517295461,
      "creation_date": 1517250228,
      "last_edit_date": 1517295461,
      "question_id": 48507685,
      "link": "https://stackoverflow.com/questions/48507685/github-public-link-format-for-accessing-my-website",
      "title": "GitHub public link format for accessing my website"
    }
  ],
  "has_more": false,
  "quota_max": 10000,
  "quota_remaining": 9972
}
```

To get question content:

**GET** `https://api.stackexchange.com/2.2/answers/55248289?order=desc&sort=activity&site=stackoverflow&filter=5)xssibJzOo)0dwNXI-h`

Read more at 

Example response: https://meta.stackexchange.com/a/264298/446319

```json
{
items: [
{
body_markdown: "You can create render the results (payments) and use a fancy way to iterate over items instead of adding a for loop. <!-- begin snippet: js hide: false console: true babel: false --> <!-- language: lang-js --> const noGuest = 3; Array(noGuest).fill(noGuest).map(guest => { console.log(guest); }); <!-- end snippet --> Example: renderPayments(noGuest) { return Array(noGuest).fill(noGuest).map(() => { return( <View> <View><TextInput /></View> <View><TextInput /></View> <View><TextInput /></View> </View> ); } } Then use it where you want it render() { return( const { guest } = this.state; ... {this.renderPayments(guest)} ); } Hope you got the idea. If you want to understand this in simple Javascript check [**Array.prototype.fill()**][1] [1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/fill"
}
]
}
```

