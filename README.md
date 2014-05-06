scalemm
=======

Delphi ScaleMM memory manager by André Mussche

It is faster (4x!) and scales better than FastMM. Also faster (3x) than TopMM, but equal scaling.

(note: only in special tests, other tests gives other results. Generally it is (a little bit) slower in single thread situations (due to other internal structure, check and get current thread manager, less optimized, etc), but faster in (heavy) multi threaded situations :-) )

Because FastMM does not scale at all, you could use TopMM (which scales very good). But TopMM is slower than FastMM (in a simple string test).

I made a proof-of-concept to see if I could make a simple and very small and compact MM, which is not as bloated (or difficult to understand) as FastMM and TopMM, and also faster than these two. Of course it must scale on multi core CPU's.

Source code can be found at: https://code.google.com/p/scalemm/ for sync
