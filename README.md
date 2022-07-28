  
# Seamless Platform Technical Documentation

## Description

This repository contains a simple template for building
[Pandoc](http://pandoc.org/) documents; Pandoc is a suite of tools to compile
markdown files into readable files (PDF, EPUB, HTML...).

## Usage

### Installing

In order to use this makefile you will need to make sure that the following
dependencies are installed on your system:
  - GNU make
  - Pandoc
  - LuaLaTeX
  - DejaVu Sans fonts

### Folder structure

Here's a folder structure for a Seamless Platform:

```
seamless-platform/  # Root directory.
|-LICENSE
|-app/						# Folder used to store builded (output) files.
 |-apis/				#
  |-account.js			#
  |-auth.js				#
  |-form.js				#
  |-message.js			#
  |-module.js			#
  |-process.js			#
  |-task.js				#
  |-user.js				#
 |-routes 					#
  |-access-management/	#
   |-group.js           #    
   |-privilege.js		#
   |-project.js 		# 
   |-role.js			#
   |-user.js			#		
  |-admin.js			#
  |-auth.js				#
  |-builder/			#
   |-flow.js		#
   |-form.js        #
   |-menu.js        #
   |-report.js      #
  |-change-password.js	#
  |-chat/               #
   |-index.js       # 
  |-config/				#
   |-locale.js		#
  |-forgot-password.js  # 
  |-help.txt			#
  |-index.js			#
  |-index_1.js			#  
  |-masters/			#
   |-contacts.js	#
   |-customer.js	#
   |-vendor.js		#
  |-message.js          #
  |-monaco.js           #
  |-myroute.js          #
  |-profile.js          #
  |-reset-password.js   #
  |-sendmail.js         #
  |-signin.js           #
  |-signout.js          #
  |-signup.js           #
  |-ui-flow.js          #
  |-unlock-user.js      #
 |-services/               #
  |-document/           #
   |-document.exists.js	#
   |-document.get.js	#
   |-document.getSerialNumber.js #
   |-document.update.js  # 
  |-email.send.js			#
 |-templates/				#
  |-form/                 #
   |-Employee Details.js #
  |-module/               #
   |-Leave Process/      #
   |-Purchase Order Approval/   #
   |-Sales Order Approval/      #
   |-Scratch/                   #
 |-views/                         #
|-core/ 						#
 |-boot.js					#
 |-handlers/					#
  |-cookie.js				#
  |-data.parser.js			#
  |-dynaflow.js				#
  |-error.js				#
  |-events.js				#
  |-favicon.js				#
  |-headers.js				#
  |-i18n.js					#
  |-jwt.js					#
  |-license.js				#
  |-oauth.js				#
  |-pjax.js					#
  |-privilege.js			#
  |-query.parser.js			#
  |-service.js				#
  |-session.js				#
  |-token.js				#
 |-http.js						#
 |-libs/						#
  |-cache.js				#
  |-chat.js					#
  |-elasticsearch.js		#
  |-email.js				#
  |-functions.js			#
  |-locale.js				#
  |-message.js				#
  |-minidb.js				#
  |-mongodb.js				#
  |-mysql.js				#
  |-oauth-model.js			#
  |-sqlite.js				#
  |-user.js					#
 |-user.js						#
 |-microservice.js				#
 |-open.js						#
 |-render.js					#
 |-router.js					#
 |-scheduler.js					#
 |-server.js					#
 |-services/					#
  |-document.js				#
  |-document_old.js         #
  |-dynaflow.js				#
  |-dynaflow_old.js			#
  |-dynaform-new.js			#
  |-dynaform.js				#
  |-dynamenu.js				#
  |-dynareport.js			#
  |-module.js				#
  |-privilege.js			#
  |-record.js				#
  |-template.js				#
 |-socket.js					#
 |-watcher.js					#
|-package-lock.json				#
|-package.json					#
|-public/						#
 |-guides/					#
  |-Account Settings/		#
   |-basic.md				#
  |-Admin Panel/			#
   |-Access Management/		#
    |-Group.md				#
	|-User.md				#
   |-Service/				#
    |-Module.md				#
  |-Getting Started/		#
   |-What is this app/		#
    |-what-is-this-app.md	#
 |-resource/					#
  |-css/					#
   |-animations.css			#
   |-bootstrap-grid.css		#
   |-bootstrap-grid.css.map	#
   |-bootstrap-grid.min.css	#
   |-bootstrap-grid.min.css.map #
   |-bootstrap-grid.rtl.css	#
   |-bootstrap-grid.rtl.min.css	#
   |-bootstrap-grid.rtl.css.map	#
   |-bootstrap-grid.rtl.min.css.map	#
   |-bootstrap-icon.css			#
   |-bootstrap-reboot.css		#
   |-bootstrap-reboot.css.map	#
   |-bootstrap-reboot.min.css	#
   |-bootstrap-reboot.min.css.map	#
   |-bootstrap-reboot.rtl.css	#
   |-bootstrap-reboot.rtl.css.map	#
   |-
```

Here's a folder structure for a Seamless Application:

```
seamless-platform/  # Root directory.
|- app/           	# Folder used to store builded (output) files.
|- public/          # Markdowns files; one for each chapter.
|- images/       	# Images folder.
|- metadata.yml  	# Metadata content (title, author...).
|- Makefile      	# Makefile used for building our documents.
```



