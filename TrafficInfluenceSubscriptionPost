package module
import (
	"context"
	"fmt"
	"net/http"
	"strings"
	"errors"
)

type TrafficInfluenceSubscriptionPostAPIService service

var (
	method   = strings.ToUpper("Post")
	postBody interface{}
	
)


func (a *TrafficInfluenceSubscriptionPostAPIService) SubscriptionPost() (TrafficInfluSub,
	*http.Response, error) {

		data := url.Values {
			"afServiceID": {"CDNCachedData"},
			"afAppID": {"CDNApp"},
			"afTransId": {"afTrans01"}
			"appReloInd": {false}
			"dnn": {"edgeLocation"}
			"snssai": { "sst: 1
				sd: 010203"
			}
			"anyUeInd": {false}
			"gpsi": {"imsi-2089300007487"}
			"ipv4Addr": {60.60.0.1}
			"flowinfo": {filter[]}
			"routes": {route[]}
			"suppFeat": {1}
		}

		path=protocol+"://"+hostname+port+basepath+"{afAppID}/subscriptions"

		headerParams := make(map[string]string)

		headerParams["Content-Type"] = contentType
		headerParams["Accept"] = contentType

		//body parameters
		postBody = &data
		r, err := a.client.prepareRequest(path, method, postBody, headerParams)
		if err != nil {
			return ret, nil, err
		}
	

		return ret, resp, nil
	}

func handleResponse(ts *TrafficInfluSub, r *http.Response, body []byte) error {
	if r.StatusCode == 201 {
		
		if err != nil {
			
		return err
	}

	return handlePostPutPatchErrorResp(r, body)
}

}
	
