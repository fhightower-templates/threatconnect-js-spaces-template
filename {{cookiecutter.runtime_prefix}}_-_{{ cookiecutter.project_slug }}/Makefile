help:
	@echo "pack 	package the app"

pack:
	# remove the old app
	rm -f {{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}.zip
	# copy the app into a new directory
	cp -r ./{{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }} {{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}_app
	# zip the app (do it recursively (-r) and ignore any hidden mac files like '_MACOSX' and '.DS_STORE' (-X))
	zip -r -X {{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}.zip {{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}_app
	# remove the copy of this package
	rm -rf {{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}_app
	@echo "App has been packaged here: {{cookiecutter.runtime_prefix}}_-_{{ cookiecutter.project_slug }}.zip"
