# OpenColab (OpenSim in Google Colab)
Biomechanical modeling in Google Colab using OpenSim

This project aims to make the life of a researcher a bit easier in dealing with Bio-mechanical models. OpenSim has got 𝐚𝐦𝐚𝐳𝐢𝐧𝐠 𝐈𝐧𝐭𝐞𝐫𝐟𝐚𝐜𝐞𝐬 including C++, Python, and Matlab. Normally, the user installs them on their PC. 

This project adds another interface where one can 𝐫𝐮𝐧 𝐧𝐞𝐮𝐫𝐨𝐦𝐮𝐬𝐜𝐮𝐥𝐨𝐬𝐤𝐞𝐥𝐞𝐭𝐚𝐥 𝐦𝐨𝐝𝐞𝐥𝐢𝐧𝐠 & 𝐬𝐢𝐦𝐮𝐥𝐚𝐭𝐢𝐨𝐧𝐬 𝐨𝐧 𝐭𝐡𝐞 𝐰𝐞𝐛 (particularly on 𝐆𝐨𝐨𝐠𝐥𝐞 𝐂𝐨𝐥𝐚𝐛). You can imagine 𝐆𝐨𝐨𝐠𝐥𝐞 𝐃𝐨𝐜𝐬 (𝐨𝐧 𝐭𝐡𝐞 𝐰𝐞𝐛) 𝐯𝐬. 𝐌𝐢𝐜𝐫𝐨𝐬𝐨𝐟𝐭 𝐖𝐨𝐫𝐝 (𝐨𝐧 𝐚 𝐏𝐂).

𝐆𝐨𝐨𝐠𝐥𝐞 𝐂𝐨𝐥𝐚𝐛: 
"𝐂𝐨𝐥𝐚𝐛𝐨𝐫𝐚𝐭𝐨𝐫𝐲, 𝐨𝐫 "𝐂𝐨𝐥𝐚𝐛" for short, allows you to write and execute Python in your browser, 𝐰𝐢𝐭𝐡 𝐙𝐞𝐫𝐨 𝐜𝐨𝐧𝐟𝐢𝐠𝐮𝐫𝐚𝐭𝐢𝐨𝐧 𝐫𝐞𝐪𝐮𝐢𝐫𝐞𝐝, 𝐅𝐫𝐞𝐞 𝐚𝐜𝐜𝐞𝐬𝐬 𝐭𝐨 𝐆𝐏𝐔𝐬, 𝐄𝐚𝐬𝐲 𝐬𝐡𝐚𝐫𝐢𝐧𝐠. Whether you're a student, a data scientist, or an AI researcher, Colab can make your work easier. Watch Introduction to Colab to learn more, or just get started below! https://colab.research.google.com/ "

If you are new to modeling, or even an expert in computational and human/animal movement science, you may have to deal with the installation of several packages, set up a new environment on your computer which usually keeps you away from the actual research.


In this project, we use Google Cloud (esp. Google Colab notebooks) and 𝐢𝐧𝐬𝐭𝐚𝐥𝐥 𝐎𝐩𝐞𝐧𝐒𝐢𝐦 via Anaconda Cloud easily (<𝟕𝐦𝐢𝐧) so that we can use it without any issue at any computer, collaborate with others and share models fast without even a need to install OpenSim on your computer. 𝒀𝒐𝒖 𝒋𝒖𝒔𝒕 𝒏𝒆𝒆𝒅 𝒕𝒐 𝒉𝒂𝒗𝒆 𝒂𝒄𝒄𝒆𝒔𝒔 𝒕𝒐 𝒕𝒉𝒆 𝒊𝒏𝒕𝒆𝒓𝒏𝒆𝒕 𝒂𝒏𝒅 𝑮𝒎𝒂𝒊𝒍 𝒂𝒄𝒄𝒐𝒖𝒏𝒕. The 𝐢𝐧𝐢𝐭𝐢𝐚𝐥 𝐬𝐞𝐭𝐮𝐩 𝐰𝐨𝐮𝐥𝐝 𝐭𝐚𝐤𝐞 <𝟏 𝐦𝐢𝐧. 

That is it! Enjoy OpenColabing!

We also created several 𝐯𝐢𝐝𝐞𝐨 𝐭𝐮𝐭𝐨𝐫𝐢𝐚𝐥𝐬 (e.g. https://youtu.be/iEjd7OSOitg) to learn Google Colab (basic python programming on the web) and OpenColab (𝐎𝐩𝐞𝐧𝐒𝐢𝐦 + 𝐆𝐨𝐨𝐠𝐥𝐞 𝐂𝐨𝐥𝐚𝐛): www.tinyurl.com/xukhmnez   


𝐇𝐨𝐰 𝐎𝐩𝐞𝐧𝐂𝐨𝐥𝐚𝐛 𝐰𝐨𝐫𝐤𝐬 𝐚𝐧𝐝 𝐡𝐨𝐰 𝐝𝐨 𝐰𝐞 𝐯𝐚𝐥𝐢𝐝𝐚𝐭𝐞 𝐢𝐭?

The image below shows how we developed and validated OpenColab. As mentioned, the Conda package was developed to install OpenSim on Colab. For validation, we compared the GUI results (for Scaling, IK, ID, RRA, SO, and CMC) with OpenColab results. The outcomes matched very well. 

𝐍𝐨𝐭𝐞𝐛𝐨𝐨𝐤𝐬:
To download the latest Ipython notebook (OpenColab.ipynb), please visit Github:
https://github.com/hmok/OpenColab 

𝐇𝐨𝐰 𝐭𝐨 𝐬𝐞𝐭 𝐮𝐩 𝐢𝐧 <𝟏𝐦𝐢𝐧 𝐚𝐧𝐝 𝐫𝐮𝐧 𝐢𝐧𝐯𝐞𝐫𝐬𝐞 𝐩𝐫𝐨𝐛𝐥𝐞𝐦 𝐢𝐧 𝐎𝐩𝐞𝐧𝐂𝐨𝐥𝐚𝐛?
Please follow the following steps to start running OpenSim simulations in < 1 min. 
Go to this website: https://colab.research.google.com/

a)	Upload the following file from Supplementary Material 2: “OpenColab.ipynb“ or from this link https://github.com/hmok/OpenColab/blob/main/OpenColab.ipynb

b)	Wait till the file is loaded. 

c)	Press Ctrl+F9 or Runtime ---> Run all (setup finished in < 1 min)

d)	No action needed by the user: OpenSim will be installed (5-7 min)

e)	The simulations will generate the results of this paper.


If you are interested in contributing, please feel free to reach out at 𝐦𝐨𝐤𝐡𝐭𝐚𝐫𝐳𝐚𝐝𝐞𝐡 𝐃𝐎𝐓 𝐡𝐨𝐬𝐬𝐞𝐢𝐧 𝐀𝐓 𝐆𝐦𝐚𝐢𝐥 𝐃𝐎𝐓 𝐜𝐨𝐦.

Please cite the following:
Mokhtarzadeh, Hossein, Fangwei Jiang, Shengzhe Zhao, and Fatemeh Malekipour. 2021. “Opencolab Project: Opensim in Google Colaboratory to Explore Biomechanics on the Web.” engrXiv. September 30. doi:10.31224/osf.io/f8a3h.

<img alt="" src="https://github.com/hmok/OpenColab/blob/main/Fig1_6Jun21.png?raw=true"/>





