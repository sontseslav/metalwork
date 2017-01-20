/**
 * Created by Stanislav Khvalinsky on 18.12.16.
 * Covered by GNU LESSER GENERAL PUBLIC LICENSE
 * For more detais please refer to official GNU site: https://www.gnu.org/licenses/lgpl-3.0.en.html
 */
var app = angular.module('validate', ['ngMask']);
app.controller('validateCtrl', function ($scope) {
  $scope.contact = {
    u_name: document.getElementById("id_u_name").getAttribute("value"), 
    from_email: document.getElementById("id_from_email").getAttribute("value"), 
    u_tel: document.getElementById("id_u_tel").getAttribute("value"), 
    message: "", 
    image: ""};
    $scope.isInvalid = '0';
    $scope.errorMsg = '';
    $scope.contact.image = function (files) {
      $scope.isInvalid = '0';
      $scope.errorMsg = '';
      var fileList = files.files;
      if (fileList.length){
        $scope.validForm.$invalid = false;
        if (fileList.length > 3) {
          $scope.isInvalid = '1';
          $scope.errorMsg = 'Слишком много файлов';
          $scope.validForm.$invalid = true;
        } else {
          for (var i = 0; i < fileList.length; i++) {
            if (fileList[i].size > 2621440 || !fileList[i].type.match(/^image\/((jpe?g)|(gif)|(png))$/)) {
              $scope.isInvalid = '1';
              $scope.errorMsg = 'Не подходит тип или размер файла';
              $scope.validForm.$invalid = true;}
            }
          }
        }
      };
      $scope.isSet = function () {
        return $scope.isInvalid == '1';
      };
    }
  );
  app.directive('emailCheck', function () {
    return {
      restrict: "C",
      require: 'ngModel',
      link: function (scope, element, attr, emailCtrl) {
        function validator(mail) {
          if (/^(([^<>()[\]\\.,;:\s@\"]+(\.[^<>()[\]\\.,;:\s@\"]+)*)|(\".+\"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/.test(mail) || (!mail)) {
            emailCtrl.$setValidity('isVerified', true);
          } else {
            emailCtrl.$setValidity('isVerified', false);
          }return mail;
        }
        emailCtrl.$parsers.push(validator);
      }
    };
  });
  app.directive('isChanged', function () {
    return {
      restrict: 'A',link: function (scope, element, attrs) {
        var onChangeHandler = scope.$eval(attrs.isChanged);
        element.bind('change', function () {
          scope.$apply(function () {
            var files = element[0], files;
            if (files) {
              onChangeHandler(files);
            }
          });
        });
      }
    };
  });
