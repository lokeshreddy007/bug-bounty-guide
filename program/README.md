# Picking a right Program

Bug bounty programs: are they all the same? Finding the right program to target is the first step to becoming a successful bug 
bounty hunter.

## Things to consider selecting a bug bounty program

1. Asset Types
2. Bug Bounty Platforms
3. Scope
4. Payouts
5. Response Times
6. Private Programs


### Asset Types

In the context of a bug bounty program, an asset is an application, website, or product that you can hack. There are different types of assets, each with its own characteristics, requirements, and pros and cons. After considering these differences, you should choose a program with assets that play to your strengths, based on your skill set, experience level, and preferences.

#### Examples

##### 1. Social Sites and Applications

Social applications need to manage interactions among users, as well as 
each user’s roles, privileges, and account integrity. They are typically full of 
potential for critical web vulnerabilities such as insecure direct object references (IDORs), info leaks, and account takeovers. These vulnerabilities occur 
when many users are on a platform, and when applications mismanage user 
information; when the application does not validate a user’s identity properly, 
malicious users can assume the identity of others. 
These complex applications also often provide a lot of user input 
opportunities. If input validation is not performed properly, these applications are prone to injection bugs, like SQL injection (SQLi) or cross-site 
scripting (XSS).

##### 2. General Web Applications
General web applications are also a good target for beginners. Here, I am referring to any web applications that do not involve user-to-user interaction.

They tend to be a little more difficult to hack than social applications, and their attack surface is smaller. If you’re looking for account takeovers and info leak vulnerabilities, you won’t have as much luck because there aren’t a lot of opportunities for users to interact 
with others and potentially steal others’ information.

##### 3. Mobile Applications (Android, iOS, and Windows)
Hacking mobile applications requires the skill set you’ve built from 
hacking web applications, as well as additional knowledge about the structure of mobile apps and programming techniques related to the platform. You should understand attacks and analysis strategies like certificate pinning bypass, mobile reverse engineering, and cryptography

Mobile applications are less popular among bug 
bounty hunters than web applications. However, the higher barrier of entry 
for mobile programs is an advantage for those who do participate. These 
programs are less competitive, making it relatively easy to find bugs


##### 5. APIs

Application programming interfaces (APIs) are specifications that define how 
other applications can interact with an organization’s assets, such as to 
retrieve or alter their data. 

A secure API 
implementation is key to preventing data breaches and protecting customer 
data. Hacking APIs requires many of the same skills as hacking web applications, mobile applications, and IoT applications. But when testing APIs, you 
should focus on common API bugs like data leaks and injection flaws.

##### 6. Source Code and Executables

If you have more-advanced programming and reversing skills, you can give 
source code and executable programs a try.


Hacking these programs can entail analyzing the source code of open 
source projects for web vulnerabilities and fuzzing binaries for potential 
exploits. You usually have to understand coding and computer science concepts to be successful here. You’ll need knowledge of web vulnerabilities, 
programming skills related to the project’s codebase, and code analysis 
skills. Cryptography, software development, and reverse engineering skills 
are helpful.

##### 7.Hardware and IoT
Last but not least are hardware and IoT programs. These programs ask you to 
hack devices like cars, smart televisions, and thermostats. Examples include 
the bug bounty programs of Tesla and Ford Motor Company


### Bug Bounty Platforms

Companies can host bug bounty programs in two ways: bug bounty platforms 
and independently hosted websites.

Bug bounty platforms are websites through which many companies host 
their programs. Usually, the platform directly awards hackers with reputation points and money for their results. 

1. [HackerOne](https://www.hackerone.com/)
2. Bugcrowd
3. Synack
4. Cobalt
5. Intigriti


### Scope

 A program’s scope on its policy pages specifies what and how you are allowed to hack. There are two types of scopes: asset and 
vulnerability. The asset scope tells you which subdomain, products, and applications you can hack. And the vulnerability scope specifies which vulnerabilities the company will accept as valid bugs.

For example, the company might list the subdomains of its website that are in and out of scope:

#### In-scope assets
a.example.com
b.example.com
c.example.com
users.example.com
landing.example.com

#### Out-of-scope assets
dev.example.com
test.example.com

On the other hand, assets that are listed as out of scope are off-limits to bug bounty hunters. Be extra careful and abide by the rules! Hacking an out-of-scope asset is illegal.The company will also often list the vulnerabilities it considers valid bugs:

#### In-scope vulnerabilities
All except the ones listed 
as out of scope

#### Out-of-scope vulnerabilities
Self-XSS
Clickjacking
Missing HTTP headers and other best 
practices without direct security impact
Denial-of-service attacks
Use of known-vulnerable libraries, without proof of exploitability
Results of automated scanners, without 
proof of exploitability

### Payout

When it comes to payments, you can distinguish between two types of programs: 
vulnerability disclosure programs and bug bounty programs. Vulnerability disclosure programs (VDPs) don’t pay monetary rewards, and bug bounty programs do.VDPs, or reputation-only programs, do not pay for findings but often offer rewards such as reputation points and swag. They are a great way to learn about hacking if making money is not your primary objective. Since they don’t pay, they’re less competitive, and so easier to find bugs in. You can use them to practice finding common vulnerabilities and communicating with security engineers.On the other hand, bug bounty programs offer varying amounts of monetary rewards for your findings. In general, the more severe thevulnerability, the more the report will pay


### Response Time

Finally, consider the program’s average response time. Some companies will handle and resolve your reports within a few days, while others take weeks or even months to finalize their fixes. Delays often happen because of the security team’s internal constraints, like a lack of personnel to handle reports, a delay in issuing security patches, and a lack of funds to timely reward researchers. Sometimes, delays happen because researchers have sent bad reports without clear reproduction steps. Prioritize programs with fast response times


#### Private Program

Most bug bounty platforms distinguish between public and private programs.Public programs are those that are open to all; anyone can hack and submit bugs to these programs, as long as they abide by the laws and thebug bounty program’s policies.On the other hand, private programs are open to only invited hackers. For these, companies ask hackers with a certain level of experience and a proven track record to attack the company and submit bugs to it. Private programs are a lot less competitive than public ones because of the limited number of hackers participating. Therefore, it’s much easier to find bugs in them. Private programs also often have a much faster response time, because they receive fewer reports on average


### A Quick Comparison 
| Program      | Asset type | In scope     | Payout   |Response time |
| ----------- | ----------- |------------- | -------- | ----------- | 
| HackerOne   | Social site | www.a.dev.com| $500     | 15 hr       |


## Summary of Choosing the Right Program


Bug bounties are a great way to gain experience in cybersecurity and earn extra bucks. But the industry has been getting more competitive. it’s becoming increasingly difficult for beginners to get started. 
That’s why it’s important to pick a program that you can succeed in from 
the very start

Before you develop a bug hunter’s intuition, you often have to rely on 
low-hanging fruit and well-known techniques. This means many other 
hackers will be able to find the same bugs, often much faster than you can. 
So, it’s a good idea to pick a program that more experienced bug hunters 
pass over to avoid competition. You can find these underpopulated programs in two ways: look for unpaid programs or go for programs with big 
scopes.

Try going for vulnerability disclosure programs first. Unpaid programs 
are often ignored by experience bug hunters, since they don’t pay monetary 
rewards. But they still earn you points and recognition! And that recognition might be just what you need to get an invite to a private, paid program.