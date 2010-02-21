!SLIDE

# plugins #

!SLIDE

# hello.py #

	@@@ python
	def hello(ui, repo, **opts):
	    print "hello world"

	cmdtable = {
	    "hw": (hello, [], 'hg hw'),
	}

!SLIDE code

# ~/.hgrc #

	[extensions]
	hgext.hw = /path/to/test.py

!SLIDE

## then we can ##

	$ hg hw
	hello world

!SLIDE

# summary.py #

	@@@ python
	def summary(ui, repo, **opts):
	    rev = opts.get('rev')
	    ctx = repo[rev]

	    ui.write(ctx.description() + "\n")

	cmdtable = {
	    "summary":
	        (summary,
	         [('r', 'rev', '', 'show the summary of the specified revision')],
	         'hg summary [-r REV]'),
	}

!SLIDE commandline incremental

	$ hg log
	changeset:   1:661ff8cfe198
	tag:         tip
	user:        Scott Chacon <schacon@gmail.com>
	date:        Sun Feb 21 09:39:05 2010 -0500
	summary:     second commit

	changeset:   0:80c84942c9a5
	user:        Scott Chacon <schacon@gmail.com>
	date:        Sun Feb 21 09:38:54 2010 -0500
	summary:     first commit

	$ hg summary -r 0
	first commit

	$ hg summary -r 1
	second commit

	$ hg summary -r 661ff8cfe198
	second commit

!SLIDE bullets incremental small

# inspired by git #

* bookmarks (git refs)
* fetch (git pull, ugh)
* rebase
* pager
* hgweb (git instaweb)
* revspec

