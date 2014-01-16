FontAwesomeAndroid
==================

Leverage the font awesome icon library (http://fortawesome.github.io/Font-Awesome/) in your android projects. The vector images will remain crisp and clear on all device sizes 

Based on "Font Awesome by Dave Gandy - http://fontawesome.io".

**note latest update to font awesome 4.0 breaks previous namespace convention, all string are prefixed by fa_ instead of icon_

How to include
----------
1. Add the <b>fontawesome-webfont.ttf</b> file into your assets directory
2. Add the <b>font_awesome.xml</b> file to your res folder
3. Add the two classes <b>ButtonAwesome.java</b> and <b>TextAwesome.java</b> to your package path

<a href="http://imgur.com/v2kAYHD"><img src="http://i.imgur.com/v2kAYHD.png?1" title="Hosted by imgur.com" /></a>

How to use
----------
There are two ways to use the icons 

1. XML layouts, just include the extended textview or button in your layout, set the text to the string resource icon
    
        <com.FontAwesome.Example.TextAwesome
            android:id="@+id/tvThumb"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/fa_thumbs_up"
            android:textSize="30sp" />

        <com.FontAwesome.Example.ButtonAwesome
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/fa_check" >

2. Create a view programmatically 

<pre>
TextAwesome tvFacebook = new TextAwesome(this);
tvFacebook.setText(this.getResources().getString(R.string.fa_facebook_square));
tvFacebook.setTextSize(TypedValue.COMPLEX_UNIT_SP,50);
layoutMain.addView(tvFacebook, new LayoutParams(LayoutParams.WRAP_CONTENT, LayoutParams.WRAP_CONTENT));
</pre>



<b>See the example project for more details</b>
