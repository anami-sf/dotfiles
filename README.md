# dotfiles

<div>

<div style="box-sizing: border-box; padding: 8px; font-family: Monaco, Menlo, Consolas, &quot;Courier New&quot;, monospace; font-size: 12px; color: rgb(51, 51, 51); border-top-left-radius: 4px; border-top-right-radius: 4px; border-bottom-right-radius: 4px; border-bottom-left-radius: 4px; background-color: rgb(251, 250, 248); border: 1px solid rgba(0, 0, 0, 0.15);-en-codeblock:true;">

<div>A django project is a collection of configuration and apps for a particular website. A project can contain multiple apps. An app can be in multiple projects.</div>

<div>An app is a Web application that does something – e.g., a Weblog system, a database of public records or a simple poll app.</div>

<div>Each app you write in Django consists of a Python package that follows a certain convention. Django comes with a utility that automatically generates the basic directory structure of an app</div>

<div>Complete setup with Postgres + Nginx + Gunicorn - <font style="color: rgb(108, 253, 255); --inversion-type-color:  simple;">https://www.digitalocean.com/community/tutorials/how-to-set-up-django-with-postgres-nginx-and-gunicorn-on-ubuntu-18-04</font></div>

</div>

<table style="border-collapse: collapse; min-width: 100%;"><colgroup><col style="width: 203px;"><col style="width: 212px;"><col style="width: 425px;"></colgroup>

<tbody>

<tr>

<td style="background-color: rgb(66, 107, 179); border: 1px solid rgb(53, 86, 143); width: 203px; padding: 8px;"></td>

<td style="background-color: rgb(66, 107, 179); border: 1px solid rgb(53, 86, 143); width: 212px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(0, 0, 0);">File location</span></div>

</td>

<td style="background-color: rgb(66, 107, 179); border: 1px solid rgb(53, 86, 143); width: 425px; padding: 8px;"></td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div>Create top level directory</div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ mkdir<directory-name></directory-name></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div>Save SSH Key</div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ ssh-add -k ~/.ssh/id_rsa</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create Virtual Env</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>Top level project directory</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Virtual Environment with PIPENV](evernote:///view/214637036/s532/53f89066-8136-408c-9060-6d6ed6f563ec/53f89066-8136-408c-9060-6d6ed6f563ec/)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Activate PIPENV</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ pipenv shell</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div>Create + clone github repo</div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>www.github.com</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Create respository](evernote:///view/214637036/s532/32ba9c65-24dd-4fe7-9e36-f322f165a4c5/32ba9c65-24dd-4fe7-9e36-f322f165a4c5/)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Install django</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ <span style="--inversion-type-color: simple; color: rgb(0, 150, 255);">pipenv install</span> django</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(0, 0, 0); font-weight: bold;">Create</span> <span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Django</span> <span style="--inversion-type-color:  simple; color: rgb(0, 0, 0); font-weight: bold;">project</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(0, 0, 0);">Inside top level directory which includes pipfile</span></div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(0, 0, 128); font-family: &quot;Fira Mono&quot;, Consolas, Menlo, Monaco, &quot;Courier New&quot;, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: no-common-ligatures; font-weight: bold;">$</span> <span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(12, 75, 51); font-family: &quot;Fira Mono&quot;, Consolas, Menlo, Monaco, &quot;Courier New&quot;, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: no-common-ligatures;">django-admin startproject <mysite_project>.</mysite_project></span></div>

<div><span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px;"></span></div>

<div><span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(12, 75, 51); font-family: &quot;Fira Mono&quot;, Consolas, Menlo, Monaco, &quot;Courier New&quot;, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: no-common-ligatures;">** The dot a the end specifies to start the new project into the current directory instead of another folder</span></div>

<div><span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px;"></span></div>

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_9.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div>django file structure</div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[https://docs.djangoproject.com/en/3.0/intro/tutorial01/#creating-a-project](https://docs.djangoproject.com/en/3.0/intro/tutorial01/#creating-a-project)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Apply migration</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ python3 manage.py migrate</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Start server</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(0, 0, 0);">project’s root directory</span></div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ <span style="--inversion-type-color: simple; color: rgb(0, 150, 255);">python3 manage.py</span> runserver 0.0.0.0:8000</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Go to local website</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>Browser</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[http://127.0.0.1:8000/](http://127.0.0.1:8000/)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create an app</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>Project Root directory</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(0, 0, 128); font-family: &quot;Fira Mono&quot;, Consolas, Menlo, Monaco, &quot;Courier New&quot;, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: no-common-ligatures; font-weight: bold;">$</span> <span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(12, 75, 51); font-family: &quot;Fira Mono&quot;, Consolas, Menlo, Monaco, &quot;Courier New&quot;, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: no-common-ligatures;">python3</span> [manage.py](http://manage.py/) <span style="font-size: 14px; white-space: pre-wrap; overflow-wrap: break-word; text-rendering: optimizeSpeed; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(12, 75, 51); font-family: &quot;Fira Mono&quot;, Consolas, Menlo, Monaco, &quot;Courier New&quot;, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: no-common-ligatures;">startapp<app_name_api></app_name_api></span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Mount app</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>project/settings.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_2.png)</div>

<div>‘<app_name>.apps.<classname>’</classname></app_name></div>

<div>*The ClassName is found in app’s apps.py file</div>

<div>from jobs/app.py find the name of the config class to add to ‘INSTALEED_APPS in the settings.py file.</div>

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_1.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Install rest framework</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>$ <span style="--inversion-type-color: simple; color: rgb(0, 150, 255);">pipenv install</span></div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>djangorestframework</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Mount rest_framework</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>project/settings.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>![](1.%20Quick%20Start.html.resources/DFE225F7-9432-41FE-A2EB-8EFF9B042448.png)</div>

<div>‘rest_framework’,</div>

<div>![](1.%20Quick%20Start.html.resources/A438677B-468D-431E-8664-7FB2E8022388.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Specify where media files should live</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>bottom of settings.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Start server</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(0, 0, 0);">project’s root directory</span></div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="--inversion-type-color: simple; color: rgb(0, 150, 255);">python3 manage.py</span> runserver 0.0.0.0:8000</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Go to local website</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>Browser</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>http://127.0.0.1:8000/</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Migrate changes</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ python3 manage.py migrate</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Create a db (psql)</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ createdb<db_name></db_name></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Connect database</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(0, 92, 197); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">DATABASES</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">=</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">{</span></span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;"></span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">default</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">: {</span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;"></span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">ENGINE</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">:</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">django.db.backends.postgresql</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">,</span></span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;"></span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">NAME</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">:</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">catcollector</span><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">,</span></span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">}</span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 11px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">}</span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create file for app_routes</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>Project’s root directory</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="font-size: 13.6px; orphans: 2; white-space: pre; widows: 2; background-color: rgb(189, 204, 219); --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace;">$ touch main_app/urls.py</span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Mount app’s URL</span> <span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">to the root projects urls file</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>inner project directory/urls.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div style="background-color: rgb(189, 204, 219); font-size: 13.6px; letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">urlpatterns</span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">=</span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">[</span></span></span></div>

<div style="background-color: rgb(189, 204, 219); font-size: 13.6px; letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">path(</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">admin/</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">, admin.site.urls),</span></div>

<div style="background-color: rgb(189, 204, 219); font-size: 13.6px; letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;"></span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(106, 115, 125); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">#</span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(106, 115, 125); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">In this case '' represents the root route</span></span></span></div>

<div style="background-color: rgb(189, 204, 219); font-size: 13.6px; letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">path(</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">, include(</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">main_app.urls</span><span style="box-sizing: border-box; font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">'</span><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">)),</span></div>

<div style="background-color: rgb(189, 204, 219); font-size: 13.6px; letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color:  simple; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">]</span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create superuser</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>Project’s root directory (Outer directory)</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="--inversion-type-color:  simple; font-size: 14px; color: rgb(5, 6, 6); font-family: SFMono-Regular;">$ python3 manage.py createsuperuser</span></div>

<div><span style="font-size: 12px; --inversion-type-color:  simple; color: rgb(5, 6, 6); font-family: SFMono-Regular;">**</span> <span style="font-size: 12px; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); color: rgb(36, 41, 46); font-family: -apple-system, system-ui, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-variant-caps: normal; font-variant-ligatures: normal;">bypass setting password by typing</span> <span style="font-size: 12px; box-sizing: border-box; background-color: rgba(27, 31, 35, 0.047); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal;">y</span> <span style="font-size: 12px; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; white-space: normal; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; background-color: rgb(255, 255, 255); color: rgb(36, 41, 46); font-family: -apple-system, system-ui, &quot;Segoe UI&quot;, Helvetica, Arial, sans-serif, &quot;Apple Color Emoji&quot;, &quot;Segoe UI Emoji&quot;, &quot;Segoe UI Symbol&quot;; font-variant-caps: normal; font-variant-ligatures: normal;">at the warning prompt.</span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create custom user model</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Custom User Model for authentication](evernote:///view/119294466/s649/3af9609e-8820-492c-a37b-92bc3f50b3a4/3af9609e-8820-492c-a37b-92bc3f50b3a4/)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Register custom user model to admin</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>app/admin.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_3.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create a Model</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Models](evernote:///view/119294466/s649/f4edfedf-db2c-4cbf-9271-88ea16d27c7b/f4edfedf-db2c-4cbf-9271-88ea16d27c7b/)</div>

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_8.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Add model to settings</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>main_app/settings.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_5.png)</div>

<div>from jobs/app.py find the name of the config class to add to ‘INSTALEED_APPS in the settings.py file.</div>

<div>![](1.%20Quick%20Start.html.resources/NSFileHandle_6.png)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create templates directory</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ touch main_app/templates</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create base template</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Template Inheritance](evernote:///view/119294466/s649/f65c90a3-e328-4e5d-b269-933e003977dd/f65c90a3-e328-4e5d-b269-933e003977dd/)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create templates directory</span></div>

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">for forms</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: visible; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; border: 0px; white-space: pre; word-break: normal; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">$ mkdir main_app/templates/main_app</span></div>

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: visible; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; border: 0px; white-space: pre; word-break: normal; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">$ touch main_app/templates/main_app/cat_form.html</span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create a View Fuction</span></div>

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">(View is equivalent to controller in exrpess)</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>polls/views.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Class Based Views ( cbv )](evernote:///view/119294466/s649/75387406-a089-4ccf-9662-18f07d122239/75387406-a089-4ccf-9662-18f07d122239/)</div>

<div>— OR —</div>

<div>[Function Views](evernote:///view/119294466/s649/25101fbc-4a3d-4a9d-96a8-b9b56179a294/25101fbc-4a3d-4a9d-96a8-b9b56179a294/)</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create static directory</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div><span style="--inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular;">**At the bottom of settings.py, there is a STATIC_URL = '/static/' variable that declares what folder within apps to look for static files in.</span></div>

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: visible; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; border: 0px; white-space: pre; word-break: normal;"></span></div>

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: visible; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; border: 0px; white-space: pre; word-break: normal; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">$ mkdir main_app/static</span></div>

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: visible; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; border: 0px; white-space: pre; word-break: normal; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">$ mkdir main_app/static/css</span></div>

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: visible; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; border: 0px; white-space: pre; word-break: normal; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">$ touch main_app/static/css/style.css</span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">ConfigRoot route</span></div>

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">(boiler plate started code)</span></div>

<div>[Routes](evernote:///view/119294466/s649/2a38e6a5-752b-4578-92e8-2b3878f0696d/2a38e6a5-752b-4578-92e8-2b3878f0696d/)</div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;">

<div>main_app/urls.py</div>

</td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>[Routes](evernote:///view/119294466/s649/2a38e6a5-752b-4578-92e8-2b3878f0696d/2a38e6a5-752b-4578-92e8-2b3878f0696d/)</div>

<div>**![](1.%20Quick%20Start.html.resources/NSFileHandle_4.png) **</div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">from</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">django.urls</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">import</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">path</span></span></span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">#The views module hold controller actions</span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">from</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">.</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">import</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">views</span></span></span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">urlpatterns</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="box-sizing: border-box; --inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(215, 58, 73); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">=</span><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">[</span></span></span></div>

<div style="background-color: rgb(189, 204, 219); letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="--inversion-type-background-color:  simple; --inversion-type-color:  simple; font-size: 12px; color: rgb(5, 6, 6); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">]</span></div>

<div style="background-color: rgb(189, 204, 219); font-size: 13.6px; letter-spacing: normal; orphans: 2; widows: 2; word-spacing: 0px; --inversion-type-background-color:  simple; --inversion-type-color:  simple;"><span style="font-size: 13.6px; --inversion-type-background-color: simple; --inversion-type-color: simple;"></span></div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192); font-weight: bold;">Create Dir for static files</span> <span style="--inversion-type-color:  simple; color: rgb(0, 0, 0); font-weight: bold;">(css, js etc)</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>$ mkdir main_app/static</div>

<div>$ mkdir main_app/static/css</div>

</td>

</tr>

<tr>

<td style="background-color: rgb(234, 234, 234); border: 1px solid rgb(187, 187, 187); width: 203px; padding: 8px;">

<div><span style="--inversion-type-color:  simple; color: rgb(111, 255, 192);">Load static files</span></div>

</td>

<td style="background-color: rgb(115, 115, 115); border: 1px solid rgb(92, 92, 92); width: 212px; padding: 8px;"></td>

<td style="width: 425px; padding: 8px; border: 1px solid;">

<div>{% load static %}</div>

<div>In the base template headed</div>

<div><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;"><</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(34, 134, 58); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">link</span> <span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(111, 66, 193); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">rel</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">=</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">"</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">stylesheet</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">"</span> <span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(111, 66, 193); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">type</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">=</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">"</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">text/css</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">"</span> <span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(111, 66, 193); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">href</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">=</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">"</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">{% static 'css/style.css' %}</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(3, 47, 98); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">"</span><span style="box-sizing: border-box; font-size: 13.6px; overflow-wrap: normal; background-color: rgb(246, 248, 250); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; overflow: auto; word-break: normal; letter-spacing: normal; orphans: 2; text-indent: 0px; text-transform: none; widows: 2; word-spacing: 0px; -webkit-text-stroke-width: 0px; color: rgb(36, 41, 46); font-family: SFMono-Regular, Consolas, &quot;Liberation Mono&quot;, Menlo, Courier, monospace; font-variant-caps: normal; font-variant-ligatures: normal; line-height: 1.45;">></span></div>

</td>

</tr>

</tbody>

</table>

</div>
