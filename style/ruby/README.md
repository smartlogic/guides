Ruby
====

We defer to [bbatsov's Ruby Style Guide](bbatsov/ruby-style-guide) with the following notable exceptions:

* Avoid single-line format for class definitions with no body <sup>[[contrasting link](bbatsov/ruby-style-guide#single-line-classes)]</sup>

  ```Ruby
  # good
  class FooError < StandardError
  end

  # okish
  class FooError < StandardError; end

  # bad
  FooError = Class.new(StandardError)
  ```

* Avoid single-line format for method definitions with no body <sup>[[contrasting link](bbatsov/ruby-style-guide#no-single-line-methods)]</sup>

  ```Ruby
  # good
  def no_op
  end

  # bad
  def no_op; end
  ```
