coq: Makefile.coq
	$(MAKE) -f Makefile.coq

clean:
	if [ -e Makefile.coq ] ; then $(MAKE) -f Makefile.coq cleanall ; fi
	rm -f Makefile.coq Makefile.coq.conf

Makefile.coq: Makefile _CoqProject.coq_makefile
	$(COQBIN)coq_makefile -f _CoqProject.coq_makefile -o Makefile.coq
