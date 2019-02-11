GITHUB_NAME = jamesblockk

deploy :
	rm -rf public
	git clone https://github.com/$(GITHUB_NAME)/$(GITHUB_NAME).github.io.git
	mv $(GITHUB_NAME).github.io public
	hugo
	cd public/ && git add . 
	cd public/ && git commit -m "[ToDo] update" 
	cd public/ && git push 