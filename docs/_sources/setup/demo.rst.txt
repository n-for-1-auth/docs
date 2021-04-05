.. _demo:

********************************************************************
N-for-1 Auth's Email Authentication Demo
********************************************************************


Setup
*************
We provide AWS instances for the demo. The key to the instances is provided here: `demo key <https://drive.google.com/drive/folders/19mUpv8Ls6karS3KIxsRxJctKbBc3viFX?usp=sharing>`_.

Once you download the key, go to the directory where the key is located and you can ssh to the instances as follows.


``ssh -i demo.pem ubuntu@52.43.71.13`` to access the instance.

Once in the instances, execute ``./run_demo.sh <email>`` on each instance to run the demo. ``<email>`` is the email address that you want the authentication email to be sent to. For example, if you want the email to be sent to ``nforoneauth@gmail.com``, then execute
``./run_demo.sh nforoneauth@gmail.com``.

Once the program finishes execution, you can check your email to see that you received the email successfully. If the email does not show up in the main inbox, please check the spam folder as well.




