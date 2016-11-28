# Model
## Validation
1. validation list :property
- validates_presence_of
e.g. validates_presence_of :name 

- validates_numbericality_of
e.g. validates_numbericality_of :total

- validates_uniqueness_of
e.g. validates_uniqueness_of :username

- validates_confirmation_of
e.g. validates_confirmation_of :password

- validates_acceptance_of
validates_acceptance_of :terms_of_service

- validates_lenght_of :property, minimum: number, maximum: number
e.g validates_lenght_of :description, minimum: 50, maximum: 250

- validates_format_of :property, with: /regex/i
e.g validates_format_of :email, with: /[a-z0-9]{3,100}@[a-z0-9]\.com/i

- validates_inclusion_of
e.g validates_inclusion_of :year, in: 2010..2050

- validates_exclusion_of
e.g validates_exclusion_of :year, in: 1990..2000,
    message: "Year was in the past!"
    