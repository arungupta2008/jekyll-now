---
id: 31
title: Solution of Taddy and Tracy Competition
date: 2012-07-14T19:06:00+00:00
author: Arun
layout: post
guid: http://arungupta.co.in/blog/?p=31
permalink: /?p=31
blogger_blog:
  - arungupta1.blogspot.com
blogger_permalink:
  - /2012/07/solution-of-taddy-and-tracy-competition.html
dsq_thread_id:
  - "2031298181"
categories:
  - Uncategorized
---
<div dir="ltr" style="text-align: left;" trbidi="on">
  <a href="http://arungupta1.blogspot.in/2012/07/tracy-and-taddy-competition-algo.html">http://arungupta1.blogspot.in/2012/07/tracy-and-taddy-competition-algo.html</a></p> 
  
  <p>
    I have Written this code by myself so please go through this &#8230;&#8230;
  </p>
  
  <p>
    <span style="font-family: 'Courier New', Courier, monospace;">import java.util.*;</span><br /><span style="font-family: 'Courier New', Courier, monospace;">import java.lang.*;</span><br /><span style="font-family: 'Courier New', Courier, monospace;">import java.io.*;</span><br /><span style="font-family: 'Courier New', Courier, monospace;">public class AStringGame {</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><br /></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><br /></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>public static void main (String [] args)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>HashMap hm = new HashMap(); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>String turn = new String(&#8220;Taddy&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>Scanner sc  = new Scanner(System.in);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int test_case = sc.nextInt();</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>Set set = hm.entrySet(); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//bool last = true;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>Iterator ik = set.iterator(); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int who = 0; // 0 teddy  1  1 tracy</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int left = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>for(int i = 0 ; i<test_case ; ++i)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//String arr = new String(&#8220;array&#8221;+i+&#8221;string&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;\n&#8221;+arr);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//int &#8221; arr&#8221;[] = new int[20];</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>String input = sc.next();</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span> int len =input.length();</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>char[] iArray = input.toCharArray();</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int inputs = sc.nextInt();</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>for(int j = 0 ; j< inputs ; ++j)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>String arr = new String(&#8220;array&#8221;+i+&#8221;:&#8221;+j+&#8221;string&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;\n&#8221;+arr);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>hm.put(arr,new String( sc.next())); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(hm.get(arr));</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span> String in =  (String) hm.get(arr);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int lenn = in.length();</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;:::::::&#8221;+lenn);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>who = 0 ;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int t = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int ine = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>char[] aArray = in.toCharArray();</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int start = 0 , end = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>for(int k = 0 ; k <len; ++k)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if(iArray[k] == aArray[0])</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int counter = k;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>start = k;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><br /></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>while(t < lenn)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if(iArray[counter] == aArray[t])</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;startinput:&#8221;+counter+&#8221;\t:check string &#8220;+t   );</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>who = 1;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>end = counter;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if((lenn -1) ==(t) )</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;Hey i am also here in if  &#8220;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;\nSome 1 Won&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>t =9898;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>left = inputs -1;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;Left *********************:&#8221;+left);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if(ine == 0)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>turn = &#8220;Tracy&#8221;;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>ine =  1;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}else</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>turn = &#8220;Taddy&#8221;;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>ine = 0;<span style="white-space: pre;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>for(int gg = start ; gg <= end ;++gg)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>iArray[gg] = &#8216;\0&#8217;;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>break; </span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;Hey i am also here in if  &#8220;); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.printf(&#8220;\nInside\n&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>++counter;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>++t;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>else if(t< lenn)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;\nI am also here \n&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;\n Some one is going to looseclea&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>t =0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>counter = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>who = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//left = left +1;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>break;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>} </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if(t == (len-1) )</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{   break;   }<span style="white-space: pre;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}<span style="white-space: pre;"> </span></span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if(t == (len-1) )</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{   break;   }</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>if(who == 0)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>int oo = 0;</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//System.out.println(&#8220;Success Success&#8221;);</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span> /*while(ik.hasNext()) { </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>//Map.Entry me = (Map.Entry)ik.next(); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>System.out.print(hm.getKey() + &#8220;: &#8220;); </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>System.out.println(hm.getValue()); </span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>} */</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><br /></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><br /></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>/*if ((left%2) == 0)</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>{</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>System.out.println(&#8220;Tracy&#8221;);<span style="white-space: pre;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>else </span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>System.out.println(&#8220;Taddy&#8221;);</span><br /><span style="font-family: 'Courier New', Courier, monospace;">*/</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>System.out.println(&#8220;\n&#8221;+turn);</span><br /><span style="white-space: pre;"><span style="font-family: 'Courier New', Courier, monospace;"> </span></span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;"><span style="white-space: pre;"> </span>}</span><br /><span style="font-family: 'Courier New', Courier, monospace;">}</span>
  </p>
</div>