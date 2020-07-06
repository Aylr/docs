
---
title: "GetAuthorizationToken"
title_tag: "Function GetAuthorizationToken | Module ecr | Package AWS"
meta_desc: "Explore the GetAuthorizationToken function of the ecr module, including examples, input properties, output properties, and supporting types. The ECR Authorization Token data source allows the authorization token, proxy endpoint, token expiration date, user name and password to be retrieved for an ECR repository."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

The ECR Authorization Token data source allows the authorization token, proxy endpoint, token expiration date, user name and password to be retrieved for an ECR repository.

{{% examples %}}
## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}

{{% example csharp %}}
```csharp
using Pulumi;
using Aws = Pulumi.Aws;

class MyStack : Stack
{
    public MyStack()
    {
        var token = Output.Create(Aws.Ecr.GetAuthorizationToken.InvokeAsync());
    }

}
```

{{% /example %}}

{{% example go %}}
```go
package main

import (
	"github.com/pulumi/pulumi-aws/sdk/v2/go/aws/ecr"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		_, err := ecr.GetAuthorizationToken(ctx, nil, nil)
		if err != nil {
			return err
		}
		return nil
	})
}
```

{{% /example %}}

{{% example python %}}
```python
import pulumi
import pulumi_aws as aws

token = aws.ecr.get_authorization_token()
```

{{% /example %}}

{{% example typescript %}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const token = pulumi.output(aws.ecr.getAuthorizationToken({ async: true }));
```

{{% /example %}}

{{% /examples %}}


## Using GetAuthorizationToken {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getAuthorizationToken<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/ecr/#GetAuthorizationTokenArgs">GetAuthorizationTokenArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/aws/ecr/#GetAuthorizationTokenResult">GetAuthorizationTokenResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">function </span> get_authorization_token(</span>registry_id=None<span class="p">, </span>opts=None<span class="p">)</span></code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetAuthorizationToken<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/v2/go/aws/ecr?tab=doc#GetAuthorizationTokenArgs">GetAuthorizationTokenArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-aws/sdk/v2/go/aws/ecr?tab=doc#GetAuthorizationTokenResult">GetAuthorizationTokenResult</a></span>, error)</span></code></pre></div>

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetAuthorizationToken </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Ecr.GetAuthorizationTokenResult.html">GetAuthorizationTokenResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Aws/Pulumi.Aws.Ecr.GetAuthorizationTokenArgs.html">GetAuthorizationTokenArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span id="registryid_csharp">
<a href="#registryid_csharp" style="color: inherit; text-decoration: inherit;">Registry<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}AWS account ID of the ECR Repository. If not specified the default account is assumed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span id="registryid_go">
<a href="#registryid_go" style="color: inherit; text-decoration: inherit;">Registry<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}AWS account ID of the ECR Repository. If not specified the default account is assumed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span id="registryid_nodejs">
<a href="#registryid_nodejs" style="color: inherit; text-decoration: inherit;">registry<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}AWS account ID of the ECR Repository. If not specified the default account is assumed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span id="registry_id_python">
<a href="#registry_id_python" style="color: inherit; text-decoration: inherit;">registry_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}AWS account ID of the ECR Repository. If not specified the default account is assumed.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## GetAuthorizationToken Result {#result}

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="authorizationtoken_csharp">
<a href="#authorizationtoken_csharp" style="color: inherit; text-decoration: inherit;">Authorization<wbr>Token</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}Temporary IAM authentication credentials to access the ECR repository encoded in base64 in the form of `user_name:password`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="expiresat_csharp">
<a href="#expiresat_csharp" style="color: inherit; text-decoration: inherit;">Expires<wbr>At</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The time in UTC RFC3339 format when the authorization token expires.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="password_csharp">
<a href="#password_csharp" style="color: inherit; text-decoration: inherit;">Password</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}Password decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="proxyendpoint_csharp">
<a href="#proxyendpoint_csharp" style="color: inherit; text-decoration: inherit;">Proxy<wbr>Endpoint</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The registry URL to use in the docker login command.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="username_csharp">
<a href="#username_csharp" style="color: inherit; text-decoration: inherit;">User<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}User name decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="registryid_csharp">
<a href="#registryid_csharp" style="color: inherit; text-decoration: inherit;">Registry<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="authorizationtoken_go">
<a href="#authorizationtoken_go" style="color: inherit; text-decoration: inherit;">Authorization<wbr>Token</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}Temporary IAM authentication credentials to access the ECR repository encoded in base64 in the form of `user_name:password`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="expiresat_go">
<a href="#expiresat_go" style="color: inherit; text-decoration: inherit;">Expires<wbr>At</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The time in UTC RFC3339 format when the authorization token expires.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="password_go">
<a href="#password_go" style="color: inherit; text-decoration: inherit;">Password</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}Password decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="proxyendpoint_go">
<a href="#proxyendpoint_go" style="color: inherit; text-decoration: inherit;">Proxy<wbr>Endpoint</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The registry URL to use in the docker login command.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="username_go">
<a href="#username_go" style="color: inherit; text-decoration: inherit;">User<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}User name decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="registryid_go">
<a href="#registryid_go" style="color: inherit; text-decoration: inherit;">Registry<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="authorizationtoken_nodejs">
<a href="#authorizationtoken_nodejs" style="color: inherit; text-decoration: inherit;">authorization<wbr>Token</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}Temporary IAM authentication credentials to access the ECR repository encoded in base64 in the form of `user_name:password`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="expiresat_nodejs">
<a href="#expiresat_nodejs" style="color: inherit; text-decoration: inherit;">expires<wbr>At</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The time in UTC RFC3339 format when the authorization token expires.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="password_nodejs">
<a href="#password_nodejs" style="color: inherit; text-decoration: inherit;">password</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}Password decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="proxyendpoint_nodejs">
<a href="#proxyendpoint_nodejs" style="color: inherit; text-decoration: inherit;">proxy<wbr>Endpoint</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The registry URL to use in the docker login command.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="username_nodejs">
<a href="#username_nodejs" style="color: inherit; text-decoration: inherit;">user<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}User name decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="registryid_nodejs">
<a href="#registryid_nodejs" style="color: inherit; text-decoration: inherit;">registry<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="authorization_token_python">
<a href="#authorization_token_python" style="color: inherit; text-decoration: inherit;">authorization_<wbr>token</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}Temporary IAM authentication credentials to access the ECR repository encoded in base64 in the form of `user_name:password`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="expires_at_python">
<a href="#expires_at_python" style="color: inherit; text-decoration: inherit;">expires_<wbr>at</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The time in UTC RFC3339 format when the authorization token expires.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="password_python">
<a href="#password_python" style="color: inherit; text-decoration: inherit;">password</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}Password decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="proxy_endpoint_python">
<a href="#proxy_endpoint_python" style="color: inherit; text-decoration: inherit;">proxy_<wbr>endpoint</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The registry URL to use in the docker login command.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="user_name_python">
<a href="#user_name_python" style="color: inherit; text-decoration: inherit;">user_<wbr>name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}User name decoded from the authorization token.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="registry_id_python">
<a href="#registry_id_python" style="color: inherit; text-decoration: inherit;">registry_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-aws">https://github.com/pulumi/pulumi-aws</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>This Pulumi package is based on the [`aws` Terraform Provider](https://github.com/terraform-providers/terraform-provider-aws).</dd>
</dl>
