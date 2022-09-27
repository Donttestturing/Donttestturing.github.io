![Brendan](images/campus%20ID%20card%20photo.png)

# Brendan Devlin

**_Aspiring Full-stack Developer_**

**Table of Contents:**
  1. [About me:](#about-me)
  2. [Code Example](#code-example)
  3. [Hobbies and Interests](#hobbies-and-interests)
  4. [Task List](#task-list)


## About me:
 I am currently a CS student at UCSD.
 I am Microsoft Java certified and I have experience in:
 - C++
 - Python
 - Javascript.

## Code Example
A code snippet I am proud is from my CSE 100 class:
```
//given a BWTransform, invert to give orig string
string invertBWT(const string & s){
	string strToReturn = "";
	vector<int> vecL2F = last2FirstHelper(s);
	vector<BWTChar> vecToSort, vec;
	int l2f;
	string str = s.substr(0);
	
	for(int i = 0; i < s.size(); i++){	//add all letters in BWT given to each vector, one will get sorted and be the vec for the first column
		BWTChar bwtCh(str[i]);
        vecToSort.push_back(bwtCh);
        vec.push_back(bwtCh);
    }
	sort(vecToSort.begin(), vecToSort.end(), BWTCharCompare);

//beginning inversion
	for(int i = 0; i < vecL2F.size()-1; i++){		
		if(i == 0){
			l2f = vecL2F[i];
			strToReturn.insert(strToReturn.begin(), vecToSort[i].getChar());
			strToReturn.insert(strToReturn.begin(), vec[i].getChar());
		}else {
			l2f = vecL2F[l2f];
			strToReturn.insert(strToReturn.begin(), vecToSort[l2f].getChar());
		}
	}
	
	return strToReturn;
}
```
This was an extra project I did to help with the final, since it was open-code. I was able to solve the test question as quickly as I was able to enter the given BWT and run the program.


## Hobbies and Interests 
I am a big fan of all sports (Soccer, Hockey, Basketball, etc.) as well as reading novels and analyzing movies. I also a fan of poetry. I find the powerful poignancy of short sharp words very pleasing to my aesthetic sensibility. A great resource for poetry is the [Poetry Foundation](https://www.poetryfoundation.org/)

 I think science can be quite magical at times, and I think many things people consider magically can be explained with science. With that in mind, here is a powerful quote by W.B. Yeats, a poet:
 
 >The world is full of magic things, patiently waiting for our senses to grow sharper


## Task List
- [ ] Get another summer internship
- [ ] Graduate from College
- [ ] Apply to Graduate Schools



Here is a funny meme I made!
[Me and My Dad](images/meAndMyDadMeme.png)

