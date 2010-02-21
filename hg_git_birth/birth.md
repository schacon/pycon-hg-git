!SLIDE subsection

# the birth of hg and git #

!SLIDE small

	Subject:	Kernel SCM saga..
	From:	Linus Torvalds (torv...@osdl.org)
	Date:	Apr 6, 2005 8:41:46 am
	List:	org.kernel.vger.linux-kernel

	"as a number of people are already aware (and in some 
	cases have been aware over the last several weeks), 
	we've been trying to work out a conflict over BK usage 
	over the last month or two (and it feels like longer ;). 
	That hasn't been working out, and as a result, the 
	kernel team is looking at alternatives."

!SLIDE

# fraternal twins #

!SLIDE small

	commit e83c5163316f89bfbde7d9ab23ca2e25604af290
	Author: Linus Torvalds <torvalds@ppc970.osdl.org>
	Date:   Thu Apr 7 15:13:13 2005 -0700

	    Initial revision of "git", the information 
	manager from hell

!SLIDE

# 2 weeks later... #

!SLIDE small

	Subject:	Mercurial v0.1 - a minimal scalable 
	         distributed SCM
	From:	Matt Mackall (mp...@selenic.com)
	Date:	Apr 20, 2005 3:10:32 am
	List:	org.kernel.vger.linux-kernel

	...
	
	* O(1) file revision storage and retrieval with efficient delta compression
	* efficient append-only layout for rsync and http range protocols
	* bare bones commit, checkout, stat, history
	* functional enough to be self-hosting[1]
	* all in less than 600 lines of Python

!SLIDE

# April 7 / April 20 #

!SLIDE

# Why did they both survive? #

!SLIDE bullets incremental

# Why did they both survive? #

* Hg was much more complete early on
* Linus didn't like the storage model
* Matt thought Linus would cave?
