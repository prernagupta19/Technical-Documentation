  
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
   |-bootstrap-reboot.rtl.min.css	#
   |-bootstrap-reboot.rtl.min.css.map	#
   |-bootstrap-utilities.css		#
   |-bootstrap-utilities.css.map	#
   |-bootstrap-utilities.min.css	#
   |-bootstrap-utilities.min.css.map	#
   |-bootstrap-utilities.rtl.css	#
   |-bootstrap-utilities.rtl.css.map	#
   |-bootstrap-utilities.rtl.min.css	#
   |-bootstrap-utilities.rtl.min.css.map	#
   |-bootstrap.css						#
   |-bootstrap.css.map					#
   |-bootstrap.min.css					#
   |-bootstrap.min.css.map				#
   |-bootstrap.rtl.css					#
   |-bootstrap.rtl.css.map				#
   |-bootstrap.rtl.min.css				#
   |-bootstrap.rtl.min.css.map			#
   |-custom.css							#
   |-custom.rtl.css						#
   |-fonts/								#
    |-bootstrap-icons.woff				#
	|-bootstrap-icons.woff2				#
   |-help-center.css					#
  |-fonts/									#
   |-nunito/							#
    |-Nunito-Italic-VariableFont_wght.ttf	#
	|-Nunito-VariableFont_wght.ttf			#
	|-OFL.txt								#
	|-nunito.css							#
	|-static/								#
	 |-Nunito-Black.ttf					#
	 |Nunito-BlackItalic.ttf			#
	 |-Nunito-Bold.ttf					#
	 |-Nunito-BoldItalic.ttf			#
	 |-Nunito-ExtraBold.ttf				#
	 |-Nunito-ExtraBoldItalic.ttf		#
	 |-Nunito-ExtraLight.ttf			#
	 |-Nunito-ExtraLightItalic.ttf		#
	 |-Nunito-Italic.ttf				#
	 |-Nunito-LightItalic.ttf			#
	 |-Nunito-Medium.ttf				#
	 |-Nunito-MediumItalic.ttf			#
	 |-Nunito-Regular.ttf				#
	 |-Nunito-SemiBold.ttf				#
	 |-Nunito-SemiBoldItalic.ttf		#
   |-roboto/							#
    |-LICENSE.txt						#
	|-Roboto-Black.ttf					#
	|-Roboto-BlackItalic.ttf			#
	|-Roboto-Bold.ttf					#
	|-Roboto-BoldItalic.ttf				#
	|-Roboto-Italic.ttf					#
	|-Roboto-Light.ttf					#
	|-Roboto-LightItalic.ttf			#
	|-Roboto-Medium.ttf					#
	|-Roboto-MediumItalic.ttf			#
	|-Roboto-Regular.ttf				#
	|-Roboto-Thin.ttf					#
	|-Roboto-ThinItalic.ttf				#
	|-roboto.css						#
 |-images/									#
 |-js/										#
 |-libs/									#
|-workers/ 									#
 |-events.js							#
 |-socket.js							#
 |-sw.js								#
```

Here's a folder structure for a Seamless application:

```
idoc-app/  							 # Root directory.
 |-LICENSE							#
 |-app.js							#
 |-app.json							#
 |-app/								#
  |-apis/						#
  |-configs/					#
  |-flows/						#
  |-forms/						#
  |-licenses/					#
  |-privileges/					#
  |-reports/					#
  |-routes/						#
  |-services/					#
  |-templates/					#
  |-views/						#
 |-cache/							#
 |-config/							#
  |-config.js					#
   |-events.js					#
   |-license.js					#
   |-license.lic				#
   |-middlewares.js				#
   |-privilege.js				#
   |-scheduler.js				#
 |-database/						#
  |-ai-bot.db					#
  |-app.db						#
  |-app1.db						#
  |-group.db					#
  |-group1.db					#
  |-list.db						#
  |-menu.db						#
  |-module.db					#
  |-module.db					#
  |-privilege.db				#
  |-privilege1.db				#
  |-process.db					#
  |-process1.db					#
  |-project.db					#
  |-role.db						#
  |-role1.db					#
  |-user.db						#
  |-user1.db					#
 |-libs/							#
  |-email.js					#
  |-filewatcher.js				#
  |-functions.js				#
  |-message.js					#
 |-locales/							#
  |-ar.json						#
  |-bn.json						#
  |-en.json						#
  |-es.json						#
  |-fr.json						#
 |-package-lock.json				#
 |-package.json						#
 |-public/							#
  |-assets/						#
   |-css/						#
   |-images/					#
   |-js/						#
  |-manifest.json				#
  |-offline.html				#
  |-worker.js					#
 |-session/							#
 |-upload/							#


