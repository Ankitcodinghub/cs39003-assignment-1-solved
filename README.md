# cs39003-assignment-1-solved
**TO GET THIS SOLUTION VISIT:** [CS39003 Assignment 1 Solved](https://www.ankitcodinghub.com/product/compiler-laboratory-cs39003-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;113926&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS39003 Assignment 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1. Translate the following C program using GCC/Linux to the assembly language program of x86-64 (Intel 64-bit processor) without optimization.

cc -Wall -S ass1.c

C Program: ass1.c

/*

* ass1.c Generate assembly code of x86-64 and comment

*/

#include &lt;stdio.h&gt; #define MAXSIZE 100

void inst_sort(int num[],int n); int bsearch(int num[],int n,int item);

int main()

{ int n, a[MAXSIZE], item, i, loc;

printf(“Enter how many elements you want: “); scanf(“%d”, &amp;n);

printf(“Enter the %d elements: “, n); for(i = 0; i &lt; n; i++) scanf(“%d”, &amp;a[i]);

inst_sort(a,n);

printf(” Enter the item to search “); scanf(“%d”, &amp;item); loc=bsearch(a,n,item);

1

if (item == a[loc]) { printf(” %d found in position: %d “, item, loc + 1);

} else { printf(” Item is not present in the list. “);

}

return 0;

}

void inst_sort(int num[],int n)

{ int i,j,k;

for(j=1;j&lt;n;j++) { k=num[j]; for(i=j-1;i&gt;=0 &amp;&amp; k&lt;num[i];i–) num[i+1]=num[i]; num[i+1]=k;

} }

int bsearch(int a[],int n,int item)

{ int mid, top, bottom;

bottom = 1; top = n; do { mid = (bottom + top) / 2; if (item &lt; a[mid]) top = mid – 1;

else if (item &gt; a[mid]) bottom = mid + 1;

} while (item != a[mid] &amp;&amp; bottom &lt;= top); return mid; }

2. Rename the generated assembly file as ass1 roll.s (where roll is your roll number). Add comments for each of the assembly language instruction. Your comment should explain the functionality of the instruction and the connection to the original C program. Please make sure that your commented file can be compiled to generate executable file. Upload your file (ass1 roll.s) in Moodle server.

2
