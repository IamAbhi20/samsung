# samsung
(gdb) run

Starting program: /home/test/Desktop/memory 

[Thread debugging using libthread_db enabled]

Using host libthread_db library "/lib/x86_64-linux-gnu/libthread_db.so.1".



Program received signal SIGSEGV, Segmentation fault.

0x00007ffff788516b in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

1030	./libio/libioP.h: No such file or directory.

(gdb) bt

#0  0x00007ffff788516b in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#1  0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#2  0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#3  0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#4  _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

#5  0x00007ffff7887c4d in __GI__IO_puts (str=0x7ffff7d21a4e "jemalloc is being used ") at ./libio/libioP.h:1030

#6  0x00007ffff7c22e8b in malloc (size=1024) at src/jemalloc.c:2795

#7  0x00007ffff78851a5 in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/filedoalloc.c:101

#8  0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#9  0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#10 0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#11 _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

#12 0x00007ffff7887c4d in __GI__IO_puts (str=0x7ffff7d21a4e "jemalloc is being used ") at ./libio/libioP.h:1030

#13 0x00007ffff7c22e8b in malloc (size=1024) at src/jemalloc.c:2795

#14 0x00007ffff78851a5 in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/filedoalloc.c:101

#15 0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#16 0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#17 0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#18 _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

#19 0x00007ffff7887c4d in __GI__IO_puts (str=0x7ffff7d21a4e "jemalloc is being used ") at ./libio/libioP.h:1030

#20 0x00007ffff7c22e8b in malloc (size=1024) at src/jemalloc.c:2795

#21 0x00007ffff78851a5 in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/filedoalloc.c:101

#22 0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#23 0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#24 0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#25 _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

#26 0x00007ffff7887c4d in __GI__IO_puts (str=0x7ffff7d21a4e "jemalloc is being used ") at ./libio/libioP.h:1030

#27 0x00007ffff7c22e8b in malloc (size=1024) at src/jemalloc.c:2795

#28 0x00007ffff78851a5 in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/filedoalloc.c:101

#29 0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#30 0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#31 0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#32 _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

#33 0x00007ffff7887c4d in __GI__IO_puts (str=0x7ffff7d21a4e "jemalloc is being used ") at ./libio/libioP.h:1030

#34 0x00007ffff7c22e8b in malloc (size=1024) at src/jemalloc.c:2795

#35 0x00007ffff78851a5 in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/filedoalloc.c:101

#36 0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#37 0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#38 0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#39 _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

#40 0x00007ffff7887c4d in __GI__IO_puts (str=0x7ffff7d21a4e "jemalloc is being used ") at ./libio/libioP.h:1030

#41 0x00007ffff7c22e8b in malloc (size=1024) at src/jemalloc.c:2795

#42 0x00007ffff78851a5 in __GI__IO_file_doallocate (fp=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/filedoalloc.c:101

#43 0x00007ffff7895514 in __GI__IO_doallocbuf (fp=fp@entry=0x7ffff7a045c0 <_IO_2_1_stdout_>) at ./libio/libioP.h:1030

#44 0x00007ffff7892f80 in _IO_new_file_overflow (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, ch=-1) at ./libio/fileops.c:745

#45 0x00007ffff7893a9f in _IO_new_file_xsputn (n=23, data=<optimized out>, f=<optimized out>) at ./libio/libioP.h:1030

#46 _IO_new_file_xsputn (f=0x7ffff7a045c0 <_IO_2_1_stdout_>, data=<optimized out>, n=23) at ./libio/fileops.c:1197

--Type <RET> for more, q to quit, c to continue without paging--



Error 2 using strace
fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0x1), ...}) = 0

--- SIGSEGV {si_signo=SIGSEGV, si_code=SEGV_MAPERR, si_addr=0x7ffcd5dc4ff8} ---

+++ killed by SIGSEGV (core dumped) +++

Segmentation fault (core dumped)

