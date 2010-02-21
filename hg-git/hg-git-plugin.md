!SLIDE

# The Hg-Git Plugin #

!SLIDE center

# hg-git.github.com #
![](img/hg-git.jpg)

!SLIDE center
![](img/hggit-idea.png)

!SLIDE

# installing #

!SLIDE code

# easy_install hg-git #

!SLIDE code

# ~/.hgrc #

	[extensions]
	hgext.bookmarks =
	hggit =

!SLIDE

	commit 2d1a527b2489c9d10e98bcfa14ee52ca4f731db4
	Author: Augie Fackler <durin42@gmail.com>
	Date:   Tue Oct 27 22:39:45 2009 -0400

	    tests: inline unit tests into main test suite
    
	    --HG--
	    rename : unit-tests/topo-test.py => tests/test-topo-sort.py
	    rename : unit-tests/url-test.py => tests/test-url-parsing.py

!SLIDE

	commit 8247160cc0d809ab059ee4ce7f4518a7e90b0324
	Author: Sverre Rabbelier <srabbelier@google.com>
	Date:   Fri Jul 31 15:27:20 2009 -0700

	    switch object mapping to hg->git since the many to one is that direction

	    --HG--
	    extra : transplant_source : %92%D2%D0%B3%19%5E%FCK%5E%B5%3A%2B%9Cy%B7%0F%D7%2Bm%D5


!SLIDE

- Hg-Git, a case study
  - General usage (implementing a new protocol in hg plugins)
  - What does not convert bidirectionally (artifact of hg data redundancy)
    - explicit rename issues
    - plugins problems : changelists vs manifest compares

