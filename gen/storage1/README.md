<!---
DO NOT EDIT !
This file was generated automatically from 'src/mako/api/README.md.mako'
DO NOT EDIT !
-->
The `google-storage1` library allows access to all features of the *Google storage* service.

This documentation was generated from *storage* crate version *0.1.5+20150326*, where *20150326* is the exact revision of the *storage:v1* schema built by the [mako](http://www.makotemplates.org/) code generator *v0.1.5*.

Everything else about the *storage* *v1* API can be found at the
[official documentation site](https://developers.google.com/storage/docs/json_api/).
# Features

Handle the following *Resources* with ease from the central [hub](http://byron.github.io/google-apis-rs/google-storage1/struct.Storage.html) ... 

* [bucket access controls](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControl.html)
 * [*delete*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControlDeleteCall.html), [*get*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControlGetCall.html), [*insert*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControlInsertCall.html), [*list*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControlListCall.html), [*patch*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControlPatchCall.html) and [*update*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketAccessControlUpdateCall.html)
* [buckets](http://byron.github.io/google-apis-rs/google-storage1/struct.Bucket.html)
 * [*delete*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketDeleteCall.html), [*get*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketGetCall.html), [*insert*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketInsertCall.html), [*list*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketListCall.html), [*patch*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketPatchCall.html) and [*update*](http://byron.github.io/google-apis-rs/google-storage1/struct.BucketUpdateCall.html)
* [channels](http://byron.github.io/google-apis-rs/google-storage1/struct.Channel.html)
 * [*stop*](http://byron.github.io/google-apis-rs/google-storage1/struct.ChannelStopCall.html)
* default object access controls
 * [*delete*](http://byron.github.io/google-apis-rs/google-storage1/struct.DefaultObjectAccessControlDeleteCall.html), [*get*](http://byron.github.io/google-apis-rs/google-storage1/struct.DefaultObjectAccessControlGetCall.html), [*insert*](http://byron.github.io/google-apis-rs/google-storage1/struct.DefaultObjectAccessControlInsertCall.html), [*list*](http://byron.github.io/google-apis-rs/google-storage1/struct.DefaultObjectAccessControlListCall.html), [*patch*](http://byron.github.io/google-apis-rs/google-storage1/struct.DefaultObjectAccessControlPatchCall.html) and [*update*](http://byron.github.io/google-apis-rs/google-storage1/struct.DefaultObjectAccessControlUpdateCall.html)
* [object access controls](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControl.html)
 * [*delete*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControlDeleteCall.html), [*get*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControlGetCall.html), [*insert*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControlInsertCall.html), [*list*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControlListCall.html), [*patch*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControlPatchCall.html) and [*update*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectAccessControlUpdateCall.html)
* [objects](http://byron.github.io/google-apis-rs/google-storage1/struct.Object.html)
 * [*compose*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectComposeCall.html), [*copy*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectCopyCall.html), [*delete*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectDeleteCall.html), [*get*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectGetCall.html), [*insert*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectInsertCall.html), [*list*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectListCall.html), [*patch*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectPatchCall.html), [*update*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectUpdateCall.html) and [*watch all*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectWatchAllCall.html)


Upload supported by ...

* [*insert objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectInsertCall.html)

Download supported by ...

* [*get objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectGetCall.html)
* [*update objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectUpdateCall.html)
* [*insert objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectInsertCall.html)
* [*compose objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectComposeCall.html)
* [*copy objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectCopyCall.html)

Subscription supported by ...

* [*watch all objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectWatchAllCall.html)
* [*list objects*](http://byron.github.io/google-apis-rs/google-storage1/struct.ObjectListCall.html)



# Structure of this Library

The API is structured into the following primary items:

* **[Hub](http://byron.github.io/google-apis-rs/google-storage1/struct.Storage.html)**
    * a central object to maintain state and allow accessing all *Activities*
    * creates [*Method Builders*](http://byron.github.io/google-apis-rs/google-storage1/trait.MethodsBuilder.html) which in turn
      allow access to individual [*Call Builders*](http://byron.github.io/google-apis-rs/google-storage1/trait.CallBuilder.html)
* **[Resources](http://byron.github.io/google-apis-rs/google-storage1/trait.Resource.html)**
    * primary types that you can apply *Activities* to
    * a collection of properties and *Parts*
    * **[Parts](http://byron.github.io/google-apis-rs/google-storage1/trait.Part.html)**
        * a collection of properties
        * never directly used in *Activities*
* **[Activities](http://byron.github.io/google-apis-rs/google-storage1/trait.CallBuilder.html)**
    * operations to apply to *Resources*

All *structures* are marked with applicable traits to further categorize them and ease browsing.

Generally speaking, you can invoke *Activities* like this:

```Rust,ignore
let r = hub.resource().activity(...).doit()
```

Or specifically ...

```ignore
let r = hub.object_access_controls().get(...).doit()
let r = hub.default_object_access_controls().patch(...).doit()
let r = hub.object_access_controls().update(...).doit()
let r = hub.object_access_controls().list(...).doit()
let r = hub.object_access_controls().patch(...).doit()
let r = hub.default_object_access_controls().update(...).doit()
let r = hub.default_object_access_controls().insert(...).doit()
let r = hub.object_access_controls().insert(...).doit()
let r = hub.object_access_controls().delete(...).doit()
let r = hub.default_object_access_controls().get(...).doit()
```

The `resource()` and `activity(...)` calls create [builders][builder-pattern]. The second one dealing with `Activities` 
supports various methods to configure the impending operation (not shown here). It is made such that all required arguments have to be 
specified right away (i.e. `(...)`), whereas all optional ones can be [build up][builder-pattern] as desired.
The `doit()` method performs the actual communication with the server and returns the respective result.

# Usage

## Setting up your Project

To use this library, you would put the following lines into your `Cargo.toml` file:

```toml
[dependencies]
google-storage1 = "*"
```

## A complete example

```Rust
extern crate hyper;
extern crate yup_oauth2 as oauth2;
extern crate google_storage1 as storage1;
use storage1::ObjectAccessControl;
use storage1::{Result, Error};
use std::default::Default;
use oauth2::{Authenticator, DefaultAuthenticatorDelegate, ApplicationSecret, MemoryStorage};
use storage1::Storage;

// Get an ApplicationSecret instance by some means. It contains the `client_id` and 
// `client_secret`, among other things.
let secret: ApplicationSecret = Default::default();
// Instantiate the authenticator. It will choose a suitable authentication flow for you, 
// unless you replace  `None` with the desired Flow.
// Provide your own `AuthenticatorDelegate` to adjust the way it operates and get feedback about 
// what's going on. You probably want to bring in your own `TokenStorage` to persist tokens and
// retrieve them from storage.
let auth = Authenticator::new(&secret, DefaultAuthenticatorDelegate,
                              hyper::Client::new(),
                              <MemoryStorage as Default>::default(), None);
let mut hub = Storage::new(hyper::Client::new(), auth);
// As the method needs a request, you would usually fill it with the desired information
// into the respective structure. Some of the parts shown here might not be applicable !
// Values shown here are possibly random and not representative !
let mut req: ObjectAccessControl = Default::default();

// You can configure optional parameters by calling the respective setters at will, and
// execute the final call using `doit()`.
// Values shown here are possibly random and not representative !
let result = hub.object_access_controls().update(&req, "bucket", "object", "entity")
             .generation("sed")
             .doit();

match result {
    Err(e) => match e {
        Error::HttpError(err) => println!("HTTPERROR: {:?}", err),
        Error::MissingAPIKey => println!("Auth: Missing API Key - used if there are no scopes"),
        Error::MissingToken => println!("OAuth2: Missing Token"),
        Error::Cancelled => println!("Operation canceled by user"),
        Error::UploadSizeLimitExceeded(size, max_size) => println!("Upload size too big: {} of {}", size, max_size),
        Error::Failure(_) => println!("General Failure (hyper::client::Response doesn't print)"),
        Error::FieldClash(clashed_field) => println!("You added custom parameter which is part of builder: {:?}", clashed_field),
        Error::JsonDecodeError(err) => println!("Couldn't understand server reply - maybe API needs update: {:?}", err),
    },
    Ok(_) => println!("Success (value doesn't print)"),
}

```
## Handling Errors

All errors produced by the system are provided either as [Result](http://byron.github.io/google-apis-rs/google-storage1/enum.Result.html) enumeration as return value of 
the doit() methods, or handed as possibly intermediate results to either the 
[Hub Delegate](http://byron.github.io/google-apis-rs/google-storage1/trait.Delegate.html), or the [Authenticator Delegate](http://byron.github.io/google-apis-rs/google-storage1/../yup-oauth2/trait.AuthenticatorDelegate.html).

When delegates handle errors or intermediate values, they may have a chance to instruct the system to retry. This 
makes the system potentially resilient to all kinds of errors.

## Uploads and Downloads
If a method supports downloads, the response body, which is part of the [Result](http://byron.github.io/google-apis-rs/google-storage1/enum.Result.html), should be
read by you to obtain the media.
If such a method also supports a [Response Result](http://byron.github.io/google-apis-rs/google-storage1/trait.ResponseResult.html), it will return that by default.
You can see it as meta-data for the actual media. To trigger a media download, you will have to set up the builder by making
this call: `.param("alt", "media")`.

Methods supporting uploads can do so using up to 2 different protocols: 
*simple* and *resumable*. The distinctiveness of each is represented by customized 
`doit(...)` methods, which are then named `upload(...)` and `upload_resumable(...)` respectively.

## Customization and Callbacks

You may alter the way an `doit()` method is called by providing a [delegate](http://byron.github.io/google-apis-rs/google-storage1/trait.Delegate.html) to the 
[Method Builder](http://byron.github.io/google-apis-rs/google-storage1/trait.CallBuilder.html) before making the final `doit()` call. 
Respective methods will be called to provide progress information, as well as determine whether the system should 
retry on failure.

The [delegate trait](http://byron.github.io/google-apis-rs/google-storage1/trait.Delegate.html) is default-implemented, allowing you to customize it with minimal effort.

## Optional Parts in Server-Requests

All structures provided by this library are made to be [enocodable](http://byron.github.io/google-apis-rs/google-storage1/trait.RequestValue.html) and 
[decodable](http://byron.github.io/google-apis-rs/google-storage1/trait.ResponseResult.html) via *json*. Optionals are used to indicate that partial requests are responses 
are valid.
Most optionals are are considered [Parts](http://byron.github.io/google-apis-rs/google-storage1/trait.Part.html) which are identifiable by name, which will be sent to 
the server to indicate either the set parts of the request or the desired parts in the response.

## Builder Arguments

Using [method builders](http://byron.github.io/google-apis-rs/google-storage1/trait.CallBuilder.html), you are able to prepare an action call by repeatedly calling it's methods.
These will always take a single argument, for which the following statements are true.

* [PODs][wiki-pod] are handed by copy
* strings are passed as `&str`
* [request values](http://byron.github.io/google-apis-rs/google-storage1/trait.RequestValue.html) are borrowed

Arguments will always be copied or cloned into the builder, to make them independent of their original life times.

[wiki-pod]: http://en.wikipedia.org/wiki/Plain_old_data_structure
[builder-pattern]: http://en.wikipedia.org/wiki/Builder_pattern
[google-go-api]: https://github.com/google/google-api-go-client

# License
The **storage1** library was generated by Sebastian Thiel, and is placed 
under the *MIT* license.
You can read the full text at the repository's [license file][repo-license].

[repo-license]: https://github.com/Byron/google-apis-rs/LICENSE.md