SignalR-AngularJs-Wrapper
=========================

SignalR-AngularJs-Wrapper

Usage

//Hub setup SignalR 
    var hub = new Hub('tweets', {
        'firstFunction': function (data) {
            $rootScope.dataContainer.push(data);
            $rootScope.$apply();
        }, 
    }, ['hubMethod1','hubMethod2']);
