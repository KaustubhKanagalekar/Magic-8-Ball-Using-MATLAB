# Magic-8-Ball-Using-MATLAB
Users can play with this program by asking Yes-No questions and receiving a prediction. You would need to specify how many questions you would be asking, and the program will function accordingly. You would need to copy this code into MATLAB (.mlx) in order for this to run

<<
% x is asking for how many predictions the user wants
x = input('How many predictions do you want?')
%This will display the results of the prediction(s)
magic8(x)


function magic8(n_times_simulation)
%This uses a for loop that will simulate it the number of times the user
%asks for
    for i = 1:n_times_simulation
        %This program uses a random integer generator
            prediction = randi([1,20]);
            %If a certain number is generated, it is categorised into
            %different results
            if prediction == 1 || prediction == 2|| prediction == 3|| prediction == 4|| prediction == 5
                disp("Prediction: Yes Definitely")
            end 
            if prediction == 6 || prediction == 7 || prediction == 8 || prediction == 9 || prediction == 10
                disp("Prediction: Outlook Good")
            end
            if prediction == 11 || prediction == 12|| prediction == 13|| prediction == 14|| prediction == 15
                disp("Prediction: Ask Me Later")
            end
            if prediction == 16|| prediction == 17 || prediction == 18|| prediction == 19|| prediction == 20
                disp("Prediction: Outlook Bad")
            end
    end
end
<<
