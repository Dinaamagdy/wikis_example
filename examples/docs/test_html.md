## Inline html form
```inline_html
<div class="row">
    <div class="col-md-6 " id="form_container">
        <h2>Contact Us</h2>
        <p>
           Please send your message below. We will get back to you at the earliest!
        </p>
        <form role="form" method="post" id="reused_form">

            <div class="row">
                <div class="col-sm-12 form-group">
                    <label for="message">
                        Message:</label>
                    <textarea class="form-control" type="textarea" id="message" name="message" maxlength="6000" rows="7"></textarea>
                </div>
            </div>
            <div class="row">
                <div class="col-sm-6 form-group">
                    <label for="name">
                        Your Name:</label>
                    <input type="text" class="form-control" id="name" name="name" required>
                </div>
                <div class="col-sm-6 form-group">
                    <label for="email">
                        Email:</label>
                    <input type="email" class="form-control" id="email" name="email" required>
                </div>
            </div>



            <div class="row">
                <div class="col-sm-12 form-group">
                    <button type="submit" class="btn btn-lg btn-default pull-right" >Send →</button>
                </div>
            </div>

        </form>
        <div id="success_message" style="width:100%; height:100%; display:none; ">
            <h3>Posted your message successfully!</h3>
        </div>
        <div id="error_message"
                style="width:100%; height:100%; display:none; ">
                    <h3>Error</h3>
                    Sorry there was an error sending your form.

        </div>
    </div>
</div>
```


## Dynamic macro

#### html_test.hello

```
!!!dynamic_content
actor = "html_test"
method = "hello"
name = "John doe"

```


## Dynamic macro with markdown

#### html_test.hello

```
!!!dynamic_content
actor = "html_test"
method = "hello_markdown"
name = "John doe"
markdown = True
```
