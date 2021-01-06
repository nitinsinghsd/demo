# demo

Get started
Open in app
Responses (3)

To respond to this story,
get the free Medium app.
Open in app
Abhishek Gaurav
Abhishek Gaurav
over 1 year ago

I am unable to add overlay image over scratch card.
1

1
Saurabh
Saurabh
12 months ago

bro that is ok but what about coding part in which i need to get some number after scratching that will add up in total money like google pay tezz please reply

Baba
Baba
over 1 year ago

This looks good. But i want to write back end logic for this. How we can give random scratch card with ranging (0–50) rs. ?

Create Google Pay (Tez) like scratch card
Anup Kumar Panwar
Anup Kumar Panwar
Mar 24, 2019·3 min read

Image for post
Every Monday we pick up our smartphone and send ₹150 to our friends in order to earn some cashback. Cashback is a smart move to keep the user engaged in the app and maintain user retention.
For a normal user, it’s just a lottery. But are you an app developer who is amazed by the UI and want to implement the same in your app? Then you are in the right place. In this blog, I’ll tell you how can you clone Google Pay scratch card view into your app.
In this approach, we will first create a layout of our cashback card and then cover it will an overlay. This overlay can be scratched to reveal the view below it. Question: which layout supports overlapping of view? Recall your android lessons, the answer is RelativeLayout. RelativeLayout is the most suitable layout for building a scratch card in android.
STEP 1: Creating the content under scratch card
The content under the scratch view is just an image (trophy) with some text under it (You’ve won ₹899), though in my case its mostly “Better luck next time” 😂😂😂. So its XML code looks as follows:
<LinearLayout
 android:layout_width=”match_parent”
 android:layout_height=”match_parent”
 android:gravity=”center”
 android:orientation=”vertical”
 android:padding=”15dp”>
    <ImageView
     android:layout_width=”90dp”
     android:layout_height=”90dp”
     android:src=”@drawable/trophy” />
    <TextView
     android:layout_width=”match_parent”
     android:layout_height=”wrap_content”
     android:gravity=”center”
     android:padding=”10dp”
     android:text=”You’ve won\n₹899"
     android:textSize=”20sp” />
</LinearLayout>
