

# NetworkingV1beta1IngressSpec

IngressSpec describes the Ingress the user wishes to exist.
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**backend** | [**NetworkingV1beta1IngressBackend**](NetworkingV1beta1IngressBackend.md) |  |  [optional]
**rules** | [**List&lt;NetworkingV1beta1IngressRule&gt;**](NetworkingV1beta1IngressRule.md) | A list of host rules used to configure the Ingress. If unspecified, or no rule matches, all traffic is sent to the default backend. |  [optional]
**tls** | [**List&lt;NetworkingV1beta1IngressTLS&gt;**](NetworkingV1beta1IngressTLS.md) | TLS configuration. Currently the Ingress only supports a single TLS port, 443. If multiple members of this list specify different hosts, they will be multiplexed on the same port according to the hostname specified through the SNI TLS extension, if the ingress controller fulfilling the ingress supports SNI. |  [optional]



