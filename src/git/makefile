inFiles=metadata.yml preambule.md  general.md basics.md projectManagement.md branch.md merge.md fork.md

html:
	pandoc --chapters --toc -o CuisinerAvecGit.html $(inFiles) -N

pdf: pandoc -t latex --chapters --toc -o CuisinerAvecGit.pdf $(inFiles) -N
