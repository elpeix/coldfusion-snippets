coldfusion-snippets
===================

Coldfusion snippets for Sublime Text

/!\ *NOT COMPLETED*

Type the snippet shortcode and then press <kbd>Tab</kbd> to complete the snippet.

---
__cfapplication__
```html
<cfcomponent displayname="Application" output="${1:no}" hint="Handle the application.">
  
  $2

  <cffunction name="OnApplicationStart" access="public" returntype="boolean" output="${3:no}" hint="Fires when the application is first created.">
    $4
  </cffunction>


  <cffunction name="OnSessionStart" access="public" returntype="void" output="${5:no}" hint="Fires when the session is first created.">
    ${6:no}
  </cffunction>


  <cffunction name="OnRequestStart" access="public" returntype="boolean" output="${7:no}" hint="Fires when prior to page processing.">
    ${8:no}
  </cffunction>


  <cffunction name="OnRequest" access="public" returntype="void" output="${9:no}" hint="Fires after pre page processing is complete.">
    ${10:no}
  </cffunction>


  <cffunction name="OnRequestEnd" access="public" returntype="void" output="${11:no}" hint="Fires after the page processing is complete.">
    ${12:no}
  </cffunction>


  <cffunction name="OnApplicationEnd" access="public" returntype="void" output="${13:no}" hint="Fires when the application is terminated.">
    ${14:no}
  </cffunction>


  <cffunction name="onError" access="public" returntype="void" output="${15:no}">
    ${16:no}
  </cffunction>
</cfcomponent>
```

__cfargument__

```html
<cfargument name="$1" type="$2" required="$3" default="$4" hint="$5" />
```

__cfcomponent__

```html
<cfcomponent output="${1:no}">
  <cfproperty name="$2" type="$3" required="${4:yes}" default="$5" />
  
  <cffunction name="${6:init}" access="${7:public}" output="${8:yes}" returntype="$9" hint="$10">
    <cfargument name="$11" type="$12" required="${13:yes}" default="$14" hint="$15" />
    
    $16
  </cffunction>
</cfcomponent>
```

__cfdump__

´´´html
<cfdump var=#$1# label="$2" />
´´´

__cfbump-abort__

```html
<cfdump var=#$1# label="$2" /><abort />
```

__cffunction__

```html
<cffunction name="$1" access="$2" output="${3:yes}" returntype="$4" hint="$5">
  <cfargument name="$6" type="$7" required="${8:yes}" default="$9" hint="$10" />
  $11
</cffunction>
```

__cfif__

```html
<cfif $1> 
  $2
<cfelse>
  $3
</cfif>
```

__cfif-elseif__

```html
<cfif $1> 
  $2
<cfelseif $3>
  $4
<cfelse>
  $5
</cfif>
```

__cfinclude__

```html
<cfinclude template="$1" />
```

__cfloop-array__

```html
<cfloop array="#$1#" index="$2">
    $3
</cfloop>
```

__cfloop-collection__

```html
<cfloop collection="#$1#" item="$2">
    $3
</cfloop>
```

__cfloop-collection__

```html
<cfloop condition = "$1"> 
  $2
</cfloop>
```

__cfloop-condition__

```html
<cfloop condition = "$1"> 
  $2
</cfloop>
```

__cfloop-index__

```html
<cfloop index="$1" from="$2" to="$3" step="$4"> 
  $5
</cfloop>
```

__cfloop-query__

```html
<cfloop query="$1">
  $2
</cfloop>
```

__cfparam__

```html
<cfreturn $1 />
```

__cfprocessingdirective__

```html
<cfprocessingdirective pageencoding="4{1:utf-8}" />
```

__cfquery__

```html
<cfquery name="$1" datasource="#$2#" username="#$3#" password="#$4#">
  $5
</cfquery>
```

__cfqueryparam__

```html
<cfqueryparam cfsqltype="$1" value="#$2#" />

```

__cfreturn__

```html
<cfreturn $1 />
```

__cfsavecontent__

```html
<cfsavecontent variable="$1">
  <cfoutput>
    $2
  </cfoutput>
</cfsavecontent>
```

__cfset__

```html
<cfset $1 = $2 />
```

__cfsetting__

```html
<cfsetting enablecfoutputonly="${1:yes}" />
```

__cfswitch__

```html
<cfswitch expression="#$1#">
  <cfcase value="$2">
    $3
    <cfbreak />
  </cfcase>
  <cfdefaultcase>
    $4
    <cfbreak />
  </cfdefaultcase>
</cfswitch>
```

__cftransation__

```html
<cftransaction action="begin">
  $1
  <cftransaction action="commit" />
</cftransaction>
```


__cftry__

```html
<cftry>
  $1

  <cfcatch type="$2">
    $3
  </cfcatch>
</cftry>
```

__newObject__

```html
<cfset ${1:object} = new ${2:Component}(${3:initParams}) />
```


---

## TODO

> cflocation
> cfmail
> cfmailparams
> cfthrow
