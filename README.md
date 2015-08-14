Feature: Loging to Sweety Application as a Patient
  Enter the Blood readings and verify success message and
  Enter Blood readings more than 4 times and verify error message

  Background: 
    Given Login to sweety application as a patient

  Scenario: Login and Enter the Blood values  as a patient and verify the success message
    Given I navigate to "entryPage"
    When I enter blood glucose value for "4" time
    Then I verify the success  message
    And I enter blood glucose value for "1" time
    Then I verify the error message
