Ruby
====

We defer to [bbatsov's Ruby Style Guide](bbatsov/ruby-style-guide) with the following notable exceptions:

## Source Code Layout

* Avoid single-line format for class definitions with no body.
<sup>[[contrasting link](bbatsov/ruby-style-guide#single-line-classes)]</sup>

  ```Ruby
  # good
  class FooError < StandardError
  end

  # okish
  class FooError < StandardError; end

  # bad
  FooError = Class.new(StandardError)
  ```

* Avoid single-line format for method definitions with no body.
<sup>[[contrasting link](bbatsov/ruby-style-guide#no-single-line-methods)]</sup>

  ```Ruby
  # good
  def no_op
  end

  # bad
  def no_op; end
  ```

* Limit lines to 100 characters.
<sup>[[contrasting link](bbatsov/ruby-style-guide#80-character-limits)]</sup>

## Be Consistent

> If you're editing code, take a few minutes to look at the code around you and
> determine its style. If they use spaces around all their arithmetic
> operators, you should too. If their comments have little boxes of hash marks
> around them, make your comments have little boxes of hash marks around them
> too.

> The point of having style guidelines is to have a common vocabulary of coding
> so people can concentrate on what you're saying rather than on how you're
> saying it. We present global style rules here so people know the vocabulary,
> but local style is also important. If code you add to a file looks
> drastically different from the existing code around it, it throws readers out
> of their rhythm when they go to read it. Avoid this.

&mdash;[Google C++ Style Guide][google-c++]

[google-c++]: http://google-styleguide.googlecode.com/svn/trunk/cppguide.xml
