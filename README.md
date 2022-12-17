<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">

 <h3 align="center">Network Intrusion Detection</h3>
<p align="center">
  Network Intrusion Detection using Machine Learning
    <br />
    <a href="https://github.com/charafmrah/network-intrusion-detection"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/charafmrah/network-intrusion-detection/issues">Report Bug</a>
    ·
    <a href="https://github.com/charafmrah/network-intrusion-detection/issues">Request Feature</a>
  </p>
</div>

<!-- ABOUT THE PROJECT -->

## About The Project

![Product Name Screen Shot][product-screenshot]

Applying machine learning algorithms to a network dataset, which encompasses a broad range of intrusions that were simulated in a military network atmosphere. This created a way to acquire fresh TCP/IP dump information for a network by replicating a customary U.S. Air Force LAN. The LAN mirrored a realistic environment and was struck with multiple attacks. A connection is a sequence of TCP packets beginning and ending at a certain period, when data moves from a source IP address to a target IP address using a definite protocol. Each connection is identified as either ordinary or featuring a particular attack type. Each connection holds about 100 bytes.
For each TCP/IP connection, 41 features are obtained from the normal and attack data (3 qualitative and 38 quantitative features). The class variable consists of two categories: Normal and Anomalous.

The dataset used is the KDD Cup 1999 dataset, which is available at the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/KDD+Cup+1999+Data).

The dataset is also used by the [NSL-KDD](https://www.unb.ca/cic/datasets/nsl.html) dataset, which is a more recent dataset that is based on the KDD Cup 1999 dataset.

The dataset is usually used by researchers to test their intrusion & anomoly detection systems. The dataset is also used by researchers to test their machine learning algorithms.

### Dataset features descriptions:
#### Basic features of individual TCP connections:
* duration:	length (number of seconds) of the connection [continuous]
* protocol_type: type of the protocol, e.g. tcp, udp, etc. [discrete]
* service: network service on the destination, e.g., http, telnet, etc. [discrete]
* src_bytes: number of data bytes from source to destination [continuous]
* dst_bytes: number of data bytes from destination to source [continuous]
* flag: normal or error status of the connection [discrete] 
* land: 1 if connection is from/to the same host/port; 0 otherwise [discrete]
* wrong_fragment: number of "wrong" fragments [continuous]
* urgent: number of urgent packets [continuous]

#### Content features within a connection:
* hot: number of "hot" indicators [continuous]
* num_failed_logins: number of failed login attempts [continuous]
* logged_in: 1 if successfully logged in; 0 otherwise [discrete]
* num_compromised: number of "compromised" conditions [continuous]
* root_shell: 1 if root shell is obtained; 0 otherwise [discrete]
* su_attempted: 1 if "su root" command attempted; 0 otherwise [discrete]
* num_root: number of "root" accesses [continuous]
* num_file_creations: number of file creation operations [continuous]
* num_shells: number of shell prompts [continuous]
* num_access_files: number of operations on access control files [continuous]
* num_outbound_cmds: number of outbound commands in an ftp session [continuous]
* is_host_login: 1 if the login belongs to the "hot" list; 0 otherwise [discrete]
* is_guest_login: 1 if the login is a "guest login"; 0 otherwise [discrete]

#### Traffic features within a connection:
* count: number of connections to the same host as the current connection in the past two seconds [continuous]
* srv_count: number of connections to the same service as the current connection in the past two seconds [continuous]
* serror_rate: % of connections that have "SYN" errors [continuous]
* srv_serror_rate: % of connections that have "SYN" errors [continuous]
* rerror_rate: % of connections that have "REJ" errors [continuous]
* srv_rerror_rate: % of connections that have "REJ" errors [continuous]
* same_srv_rate: % of connections to the same service [continuous]
* diff_srv_rate: % of connections to different services [continuous]
* srv_diff_host_rate: % of connections to different hosts [continuous]



### Types of attacks: 
* DOS: denial-of-service, e.g. syn flood;
* R2L: unauthorized access from a remote machine, e.g. guessing password;
* U2R:  unauthorized access to local superuser (root) privileges, e.g., various "buffer overflow" attacks;
* probing: surveillance and other probing, e.g., port scanning.

The test data used in this task differs from the training data in terms of the distribution of data and the types of attacks included. This makes the task more realistic, as it reflects the idea that novel attacks are often variations of known attacks. The training data includes 24 types of attacks, while the test data includes an additional 14 types.


### Used Technologies:

- [![Python][python]][python-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->

## Contact

Charaf Mrah - [@charafmrah](https://twitter.com/charafmrah) - charaf4charaf@gmail.com

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Acknowledgments

-[UCI Machine Learning Repository - KDD Cup 1999 Data](https://archive.ics.uci.edu/ml/datasets/KDD+Cup+1999+Data)
-[Jupyter Notebook](https://jupyter.org/)
-[Pandas](https://pandas.pydata.org/)
-[Numpy](https://numpy.org/)
-[Matplotlib](https://matplotlib.org/)
-[Scikit-learn](https://scikit-learn.org/stable/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

[license-shield]: https://img.shields.io/github/license/charafmrah/network-intrusion-detection.svg?style=for-the-badge
[license-url]: https://github.com/charafmrah/network-intrusion-detection/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/charafmrah
[product-screenshot]: assets/network-intrusion.jpg
[python]: https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white
[python-url]: https://www.python.org/