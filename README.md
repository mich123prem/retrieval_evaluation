# Retrieval evaluation with python
#### Michael Preminger

## A notebook for demonstrating IR evaluation 

#### Made for the IR course MBIB4230 at Oslo Metropolitan University

### Using pytrec_eval by <a href="http://chri.stophr.be/">Christophe Van Gysel</a> <div class="cite2c-biblio"></div><div class="cite2c-biblio"></div> 
@inproceedings{VanGysel2018pytreceval,
  title={Pytrec\_eval: An Extremely Fast Python Interface to trec\_eval},
  author={Van Gysel, Christophe and de Rijke, Maarten},
  publisher={ACM},
  booktitle={SIGIR},
  year={2018},
}

## Before use:
* install pytrec_eval: 
  * The **pip install** currently does not work properly. 
  * download the repository from https://github.com/cvangysel/pytrec_eval ("clone or download"), open the zip file, and run:
    * python3 setup.py build
    * python3 setup.py install

* install the elasticsearch python client: 
  * pip install elasticsearch.




* (Registered users only) Establish a tunnel for using Oslomets elasticsearch installation
  
  * MAC and Linux: 
  
    * run: ssh -N  -L 9200:localhost:9200 s******@ark1.hioa.no -pw mbib4230
    * s****** is your student login
	*  Windows: You will need the **plink** utility to connect to our elasticsearch installation while off-campus.
	  * Download the appropriate putty package from [this site](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
	  * Run the windows installer
	  * Establish an ssh-tunnell against the ark1.oslomet.no server: (can be attached to a clickable icon)
	    * open a command window (cmd.exe)
	    * run the following: 
		  * %windir%\system32\cmd.exe /C plink -N  -L 9200:localhost:9200 s******@ark1.hioa.no -pw mbib4230
		  * s****** is your student login


## How to use
Pay particular attention to the run() function under "Utility functions"

    * It has parameters with default values (for example the query file name), that you can override when calling. 
    * Comapre a couple of calls to run down the notebook with the function definition. 



