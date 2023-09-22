# jinja_django


## Request object attributes

- {{ request.scheme }}  Output:-> http
- {{ request.path  }}  Output:-> /user/update/blog/dbms
- {{request.get_host}}  Output:-> 127.0.0.1:8000
- {{ request.META.HTTP_HOST }}  Output:-> 127.0.0.1:8000
- {{ request.build_absolute_uri }}  Output:-> http://127.0.0.1:8000/user/update/blog/dbms
- {{ request.method }}  Output:-> GET
- {{ request.META.USERNAME }}  Output:-> ACER
- {{ request.META.HTTP_USER_AGENT }}  Output:-> Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36
- {{ request.META.COMPUTERNAME}}  Output:-> DESKTOP-DSJ4LO3
- {{ request.META.COMSPEC }}  Output:-> C:\Windows\system32\cmd.exe
- {{ request.META.ENV_PROMPT }}  Output:-> (venv)
- {{ request.META.FPS_BROWSER_APP_PROFILE_STRING }}  Output:-> Internet Explorer
- {{ request.META.FPS_BROWSER_USER_PROFILE_STRING }}  Output:-> Default
- {{ request.META.HOMEDRIVE }}  Output:-> C:
- {{ request.META.HOMEPATH }}  Output:-> \Users\ACER
- {{ request.META.NUMBER_OF_PROCESSORS }}  Output:-> 4
- {{ request.META.OS }}  Output:-> Windows_NT
- {{ request.META.PATH }}  Output:-> H:\A_Django\Blog\venv\Scripts;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;
- {{ request.META.PROCESSOR_ARCHITECTURE }}  Output:-> AMD64
- {{ request.META.PROCESSOR_IDENTIFIER }}  Output:->Intel64 Family 6 Model 61 Stepping 4, GenuineIntel
- {{ request.META.SYSTEMDRIVE }}  Output:-> C:
- {{ request.META.SYSTEMROOT }}  Output:-> C:\Windows
- {{ request.META.USERDOMAIN }}  Output:-> DESKTOP-DSJ4LO3
- {{ request.META.USERDOMAIN_ROAMINGPROFILE }}  Output:-> DESKTOP-DSJ4LO3
- {{ request.META.USERPROFILE }}  Output:-> C:\Users\ACER
- {{ request.META.VIRTUAL_ENV }}  Output:-> H:\A_Django\Blog\venv
- {{ request.META.TERM_PROGRAM }}  Output:-> vscode
- {{ request.META.TERM_PROGRAM_VERSION }}  Output:-> 1.82.2
- {{ request.META.DJANGO_SETTINGS_MODULE }}  Output:-> Blog.settings
- {{ request.META.RUN_MAIN }}  Output:-> true
- {{ request.META.SERVER_NAME }}  Output:-> na1r.services.adobe.com
- {{ request.META.SERVER_PORT }}  Output:-> 8000
- {{ request.META.REMOTE_HOST }}  Output:-> 
- {{ request.META.SERVER_PROTOCOL }}  Output:-> HTTP/1.1
- {{ request.META.SERVER_SOFTWARE }}  Output:-> WSGIServer/0.2
- {{ request.META.REQUEST_METHOD }}  Output:-> GET
- {{ request.META.PATH_INFO }}  Output:-> /user/update/blog/dbms
- {{ request.META.REMOTE_ADDR }}  Output:-> 127.0.0.1
- {{ request.META.CONTENT_TYPE }}  Output:-> text/plain
- {{ request.META.HTTP_CONNECTION }}  Output:-> keep-alive
- {{ request.META.HTTP_CACHE_CONTROL }}  Output:-> max-age=0
- {{ request.META.HTTP_SEC_CH_UA }}  Output:-> "Chromium";v="116", "Not)A;Brand";v="24", "Google Chrome";v="116"
- {{ request.META.HTTP_SEC_CH_UA_MOBILE }}  Output:-> ?0
- {{ request.META.HTTP_SEC_CH_UA_PLATFORM }}  Output:-> "Windows"
- {{ request.META.HTTP_UPGRADE_INSECURE_REQUESTS }}  Output:-> 1
- {{ request.META.HTTP_COOKIE }}  Output:-> csrftoken=GWThLsAByE58mfQ9RkF8lGuMbeskpgqI; sessionid=67i17697fi1gn3gahuur6swxlkadezti; _ga=GA1.1.80804490.1695310503; _gid=GA1.1.820683412.1695310503
- {{ request.META.CSRF_COOKIE }}  Output:-> GWThLsAByE58mfQ9RkF8lGuMbeskpgqI
- {{ request.META.CSRF_COOKIE_NEEDS_UPDATE }}  Output:-> True
- {{ request.session }}  Output:-> <django.contrib.sessions.backends.db.SessionStore object at 0x000001F7BD98F340>

- {{ request.COOKIES }}  Output:-> {'csrftoken': 'GWThLsAByE58mfQ9RkF8lGuMbeskpgqI', 'sessionid': '67i17697fi1gn3gahuur6swxlkadezti', '_ga': 'GA1.1.80804490.1695310503', '_gid': 'GA1.1.820683412.1695310503'}
- {{ request.FILES}}  Output:-> <MultiValueDict: {}>
- {{ request.path_info }}  Output:-> /user/update/blog/dbms
- {{ request.resolver_match.url_name }}  Output:-> update-blog
- {{ request.resolver_match.view_name }}  Output:-> update-blog
- {{ request.resolver_match.kwargs }}  Output:-> {'slug': 'dbms'}
- {{ request.resolver_match.route }}  Output:-> user/update/blog/<str:slug>
- {{ request.resolver_match.captured_kwargs }}  Output:-> {'slug': 'dbms'}
- {{ request.is_secure }}  Output:-> False
- {{ request.get_full_path }}  Output:-> /user/update/blog/dbms
- {{ request.get_port }}  Output:-> 8000
- {{ request.headers }}  Output:-> {'Content-Length': '', 'Content-Type': 'text/plain', 'Host': '127.0.0.1:8000', 'Connection': 'keep-alive', 'Cache-Control': 'max-age=0', 'Sec-Ch-Ua': '"Chromium";v="116", "Not)A;Brand";v="24", "Google Chrome";v="116"', 'Sec-Ch-Ua-Mobile': '?0', 'Sec-Ch-Ua-Platform': '"Windows"', 'Upgrade-Insecure-Requests': '1', 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Safari/537.36', 'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7', 'Sec-Fetch-Site': 'none', 'Sec-Fetch-Mode': 'navigate', 'Sec-Fetch-User': '?1', 'Sec-Fetch-Dest': 'document', 'Accept-Encoding': 'gzip, deflate, br', 'Accept-Language': 'en-US,en;q=0.9', 'Cookie': 'csrftoken=GWThLsAByE58mfQ9RkF8lGuMbeskpgqI; sessionid=67i17697fi1gn3gahuur6swxlkadezti; _ga=GA1.1.80804490.1695310503; _gid=GA1.1.820683412.1695310503'}
