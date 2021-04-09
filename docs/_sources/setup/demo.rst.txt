.. _demo:

********************************************************************
N-for-1 Auth's Email Authentication Demo
********************************************************************


Setup
*************
We provide AWS instances for the demo. The key to the instances is provided in the shared Google folder.

Once you download the key, go to the directory where the key is located and you can ssh to the instances as follows.


Party 0: Run ``ssh -i demo.pem ubuntu@52.43.71.13`` to access the instance.

Party 1: Run ``ssh -i demo.pem ubuntu@52.36.82.224`` to access the instance.

Party 2: Run ``ssh -i demo.pem ubuntu@52.35.221.216`` to access the instance.


Once in the instances, execute ``./run_demo.sh <email>`` on each instance to run the demo. Run this script on parties 1 and 2 first and then party 0. ``<email>`` is the email address that you want the authentication email to be sent to. For example, if you want the email to be sent to ``nforoneauth@gmail.com``, then execute
``./run_demo.sh nforoneauth@gmail.com``. If no argument is provided, the default email is ``nforoneauth@gmail.com``.

Once the program finishes execution, you can check your email to see that you received the email successfully. If the email does not show up in the main inbox, please check the spam folder as well.

