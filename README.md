# Install Jupyter and Git on Android

Nowadays, many people need to work remotely but the idea of bringing everywhere a laptop
is not very easy and why should it when you have a smartphone in your pocket. 
Ok, of course it's not the same but sometimes you have to work with what you have. 

Let's dive in.

1. Install [Termux](https://play.google.com/store/apps/details?id=com.termux) from Google Play.
2. Run the following command to install Python  


  `apt install clang python python-dev fftw libzmq libzmq-dev freetype freetype-dev libpng libpng-dev pkg-config`
  
  
3. Then this command to install jupyter and the following dependencies  
    -numpy  
    -matplotlib  
    -pandas  
     I think they are enough but feel free to choose.  
     
     
  `LDFLAGS=" -lm -lcompiler_rt" pip install jupyter numpy matplotlib pandas`
    
    
4. You can check if everything is ok by typing  


  `jupyter notebook`  
  
  
  and you should see something like that in your screen  
  ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Jupyter running")  
5. Then you open your favourite browser and paste the following url

and...  
![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Jupyter localhost")  

VOILA!

Now, there is no point of installing Jupyter if you have no files to work, right?  
So, let's install git.  
Run the following command in Termux.

  `apt install git`

And that's it!  
You can now use the same commands to clone, pull, fetch etc as in your pc.

And on last thing for my fellow Scholars in Secure and Private AI Challenge.  
You can clone the notebooks by typing 

  `git clone https://github.com/udacity/deep-learning-v2-pytorch.git`
