== Stack ==

This is an easy way to use JavaScript prototypal inheritance to build a stack.

    var Stack = function(){
        return {
            push: function( e){
            
                function F(){}
                F.prototype= this;
                
                var that = new F,
                    self = this;
                    
                that.top = e;
                that.pop = function(){
                    return self;
                }
                
                return that;
            }
        };
    };

