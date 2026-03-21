# Lespion - CyberDefenders 
### Link to lab - ![Link here](https://cyberdefenders.org/blueteam-ctf-challenges/lespion/)
### Difficulty - Easy

#### In this Challenge we have a `.zip` file which have 3 files.

![Alert Screenshot](Screenshots/no1.png)

#### We have 2 imaages,1 text file. After opening the file we can see a github link.

![Alert Screenshot](Screenshots/no2.png)

#### After opening url in browser we can see a github profile 

![Alert Screenshot](Screenshots/no3.png)

#### Lets do some OSINT now !

## Q1 - File -> Github.txt: What API key did the insider add to his GitHub repositories?
#### We have to find a API key, by going Repositories section we see a repository named `project build -custom login pages` that looked suspicious to me. I opened it and saw 2 javascript files.

![Alert Screenshot](Screenshots/1.1.png)

#### After opening `Login page.js` file we found API key

![Alert Screenshot](Screenshots/1.2.png)

## Q2 - File -> Github.txt: What plaintext password did the insider add to his GitHub repositories?

#### On the same `Login page.js` page we can see password encoded with base64.

![Alert Screenshot](Screenshots/2.1.png)

#### Since it is encoded, So we'll decode it. After decoding we found plaintext password.

![Alert Screenshot](Screenshots/2.2.png)

## Q3 - File -> Github.txt: What cryptocurrency mining tool did the insider use?

#### If we see carefully in repositories list we can see xmrig repository, which in description is miner. This tells it is a cryptocurrency mining tool.
![Alert Screenshot](Screenshots/3.1.png)

#### We can see full information of tool in readme file.

![Alert Screenshot](Screenshots/3.2.png)

## Q4 - On which gaming website did the insider have an account?
#### Web searching the username we see on github can prrobably give us more websites this insider could've created account on.

![Alert Screenshot](Screenshots/4.1.png)

#### After scrolling we found the steam account of insider.

![Alert Screenshot](Screenshots/4.2.png)

![Alert Screenshot](Screenshots/4.3.png)

## Q5 - What is the link to the insider Instagram profile?

#### By websearch we also found the instagram account of insider.

![Alert Screenshot](Screenshots/5.png)

## Q6 - Which country did the insider visit on her holiday?

#### We can see few photos of insider on thier insatgram profile.
![Alert Screenshot](Screenshots/6.1.png)

#### If we do search this image on image reverse search tool like google lens or tineye or microsoft bing, we can find some information.

![Alert Screenshot](Screenshots/6.2.png)

#### After doing reverse image search we found this building in photo is situated in a city and we got the location, there's high chance that insider could've visited to this city on her holiday.

## Q7 - Which city does the insider family live in?

#### Here we have few more photos which can tell us, where insider's family live or lived.

![Alert Screenshot](Screenshots/7.1.png)

#### After reverse searching these images we found the location where insider's family live.

![Alert Screenshot](Screenshots/7.2.png)

## Q8 - File -> office.jpg: You have been provided with a picture of the building in which the company has an office. Which city is the company located in?

#### When I tried reverse image searched `office.jpg`. i couldn't found accurate answer.

#### Then I opened image and saw texts on the sign board.

![Alert Screenshot](Screenshots/8.1.png)

#### Then, I searched these text manually on web and found city where comapany is located. (I searched for moor street and found out it was loacated in birmingham and other seach locations too were pointing towards birmingham so that made it's probability much high)

![Alert Screenshot](Screenshots/8.2.png)

## Q9 - File -> Webcam.png: With the intel, you have provided, our ground surveillance unit is now overlooking the person of interest suspected address. They saw them leaving their apartment and followed them to the airport. Their plane took off and landed in another country. Our intelligence team spotted the target with this IP camera. Which state is this camera in?

#### I reverse seached this `Webcam.png` file on microsoft bing and found this image was in the megazine of a university.

![Alert Screenshot](Screenshots/9.1.png)

#### Then I opened the university's website and found the address

![Alert Screenshot](Screenshots/9.2.png)

#### Then i searched address on web and found the location.

![Alert Screenshot](Screenshots/9.3.png)

### Thanks for viewing !

#### This challenge was Threat intel category. It was very good to sharpen OSINT, information gathering skills. 

