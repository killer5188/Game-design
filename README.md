just scripts i want to use in an exam where im not allowed to take a usb stick in!!!!
https://github.com/IDSaves/2d-character-movement-script - side scroller 2d (top down i have made myself)
https://www.techwithsach.com/post/how-to-add-a-simple-countdown-timer-in-unity - time script pasted below incase website is blocked 

using System.Collections;
using UnityEngine.UI;
using UnityEngine;
using UnityEngine.SceneManagement;

public class StartGame : MonoBehaviour
{

    public float timeLeft = 3.0f;
    public Text startText; // used for showing countdown from 3, 2, 1 


    void Update()
    {
        timeLeft -= Time.deltaTime;
        startText.text = (timeLeft).ToString("0");
        if (timeLeft < 0)
        {
            //Do something useful or Load a new game scene depending on your use-case
        }
    }
} 

